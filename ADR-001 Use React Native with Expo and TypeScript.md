# ADR-001 Use react native with Expo and TypeScript

### Status

Decision accepted for Phase 2

### Context

FairShare is an Android course app for income, expenses, budgets, and charts. The team selected React Native, Expo, TypeScript, Tailwind CSS, and local SQLite.

### Decision

Build the Android client with React Native, Expo, and TypeScript. Use NativeWind for Tailwind-style classes on native components such as View, Text, and Pressable. Keep Expo managed workflow; avoid custom native modules unless required.

### Consequences

- NativeWind configuration and versions must match the chosen Expo SDK.
- Avoid adding design or animation libraries unless a screen needs them.
- Verify layouts on an Android emulator or device.
