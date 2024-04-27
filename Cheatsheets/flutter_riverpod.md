# Riverpod Flutter State Management Cheatsheet

## Basic Provider:

### Step 1:
  - Wrap `MyApp()` with `ProviderScope` widget inside `runApp()` function.
  
  ```dart
  void main() {
    runApp(
      ProviderScope(
        child: MyApp(),
      ),
    );
  }
  ```

### Step 2:
  - Change the `extends` from `StatelessWidget` to `ConsumerWidget`.
  - Add parameter `WidgetRef ref` to the build method.
  
  ```dart
  class MyApp extends ConsumerWidget {
    @override
    Widget build(BuildContext context, WidgetRef ref) {
      return Scaffold(
        // Your UI Widgets
      );
    }
  }
  ```

### Step 3:
  - Create Provider and set initial value.
  
  ```dart
  final providerName = Provider<ClassType>((ref) => Value);
  ```

### Step 4:
  - Access and modify the state.
  
  ```dart
  final somethingToGetValue = ref.watch(providerName);
  ref.read(providerName.notifier).stateChange(); // Update the state
  ```

## State Provider:
### Step 3:
   - Create Provider and set initial value.
   
   ```dart
   final stateProviderName = StateProvider<ClassType>((ref) => Value);
   ```

   - Optionally, use `autoDispose` to automatically clear state if it's not being listened to.
   
   ```dart
   final stateProviderNameWithAutoDispose = StateProvider.autoDispose<ClassType>((ref) => Value);
   ```

## Stream Provider
### Step 3:
  - Create a class for StreamRepository.
  
  ```dart
  final streamRepoProviderName = Provider<StreamRepositoryName>((ref) => StreamRepository());
  ```

  ```dart
  class StreamRepositoryName {
    Stream<ClassType> getStream() {
      return Stream.periodic(const Duration(seconds: 1), (i) => i).take(30); // Generates numbers 0-29 every second as a stream
    }
  }
  ```

### Step 4:
  - Create the provider for the stream and access it in the widget.
  
  ```dart
  final streamValueProvider = StreamProviderName((ref) {
    final streamRepo = ref.watch(streamRepoProviderName);
    return streamRepo.getStream();
  });
  ```

### Step 5: Accessing and Modifying UI:
  - Inside the build method:
  
  ```dart
  final stream = ref.watch(streamValueProvider);
  ```

  - Use `when` to handle different states:
  
  ```dart
  body: stream.when(
    data: (data) => Center(child: Text(data.toString())),
    error: (error, stackTrace) => Text(error.toString()),
    loading: () => const CircularProgressIndicator(),
  )
  ```


## Future Provider:

### Step 3:
   - Create Provider and set initial value.
   
   ```dart
   final futureProviderName = FutureProvider<ClassType>((ref) => Future.value(Value));
   ```

### Step 4:
   - Access the future and handle different states.
   
   ```dart
   final future = ref.watch(futureProviderName);
   
   body: future.when(
     data: (data) => Text(data.toString()),
     loading: () => CircularProgressIndicator(),
     error: (error, stackTrace) => Text('Error: $error'),
   )
   ```

## StreamProvider.family:

### Step 3:
   - Create a provider for a stream that depends on an argument.
   
   ```dart
   final streamProviderFamily = StreamProvider.family<ClassType, String>((ref, arg) {
     final streamRepo = ref.watch(streamRepoProviderName);
     return streamRepo.getStream(arg);
   });
   ```

### Step 4:
   - Use the provider with an argument to obtain the stream.
   
   ```dart
   final stream = ref.watch(streamProviderFamily('argument'));
   ```

## ScopedProvider:

### Step 1:
   - Wrap a part of the widget tree with a `ProviderScope`.
   
   ```dart
   ProviderScope(
     child: ScopedWidget(),
   )
   ```

### Step 2:
   - Create a provider that is scoped to a part of the widget tree.
   
   ```dart
   final scopedProviderName = ScopedProvider<ClassType>((ref) => Value);
   ```

### Step 3:
   - Access the scoped provider within the scoped widget.
   
   ```dart
   final scopedValue = ref.watch(scopedProviderName);
   ```

## AutoDispose Provider:

### Step 3:
   - Create a provider that automatically disposes its value when no longer used.
   
   ```dart
   final autoDisposeProviderName = Provider.autoDispose<ClassType>((ref) => Value);
   ```

### Step 4:
   - Access the auto-disposing provider.
   
   ```dart
   final value = ref.watch(autoDisposeProviderName);
   ```


## Basic Provider:

### Access and UI Update:
```dart
// Access
final value = ref.watch(providerName);

// UI Update
ref.read(providerName.notifier).stateChange(); // Update the state
```

## State Provider:

### Access and UI Update:
```dart
// Access
final value = ref.watch(stateProviderName);

// UI Update
value.state = newValue; // Update the state
```

## Stream Provider:

### Access and UI Update:
```dart
// Access
final stream = ref.watch(streamValueProvider);

// UI Update
body: stream.when(
  data: (data) => Center(child: Text(data.toString())),
  error: (error, stackTrace) => Text(error.toString()),
  loading: () => const CircularProgressIndicator(),
)
```

## Future Provider:

### Access and UI Update:
```dart
// Access
final future = ref.watch(futureProviderName);

// UI Update
body: future.when(
  data: (data) => Text(data.toString()),
  loading: () => CircularProgressIndicator(),
  error: (error, stackTrace) => Text('Error: $error'),
)
```

## StreamProvider.family:

### Access and UI Update:
```dart
// Access
final stream = ref.watch(streamProviderFamily('argument'));

// UI Update
body: stream.when(
  data: (data) => Center(child: Text(data.toString())),
  error: (error, stackTrace) => Text(error.toString()),
  loading: () => const CircularProgressIndicator(),
)
```

## ScopedProvider:

### Access and UI Update:
```dart
// Access
final value = ref.watch(scopedProviderName);

// UI Update
value.state = newValue; // Update the state
```

## AutoDispose Provider:

### Access and UI Update:
```dart
// Access
final value = ref.watch(autoDisposeProviderName);

// UI Update
value.state = newValue; // Update the state
```
