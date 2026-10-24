# NoteSwift · student learning app

An Expo/React Native student application for a broader learning-platform design. This public repository contains the [student app](student); the backend and teacher/admin applications described in earlier project notes are not included here.

## Source scope

The student application includes routed learning interfaces, API clients, authentication state, reusable components, and mobile assets. It uses TypeScript, Expo Router, NativeWind, Zustand, Axios, and Expo SecureStore.

The package manifest declares Expo 53, React 19, and React Native 0.79. These are source dependency versions, not a claim that the app has been upgraded to the latest SDK.

## Run the student client

```bash
cd student
npm install
npm start
```

The client needs a compatible backend. Review the [API configuration](student/api/README.md) and the API client code, then use a server address reachable from your simulator or physical device. A local backend is not supplied by this repository.

Other app scripts include `npm run android`, `npm run ios`, `npm run web`, and `npm run lint`. Native build requirements depend on the platform and enabled modules.

## Boundaries

The wider product design includes educator/admin tooling, live classes, recommendations, and offline learning. This repository alone does not establish that those services are implemented, deployed, or available. Validate each workflow against the client code and its connected backend; avoid inferring multi-tenant isolation, payment support, or offline guarantees from the original platform overview.
