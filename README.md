# React Native Android Crash on API Fetch Failure

This repository demonstrates a common issue in React Native Android applications where network errors during API data fetching lead to crashes.  The provided code shows the buggy component and its improved, error-handled version.

The bug is caused by the lack of proper error handling within the `useEffect` hook's `async` function.  The app crashes because it fails to gracefully handle `response.ok` being false or other network errors.

The solution provides comprehensive error handling, ensuring the app gracefully displays an error message to the user rather than crashing.