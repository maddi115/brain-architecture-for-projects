do this from the project directory: node tools/codebrain.mjs tree src 

for example : maddi/~/proximity-profiles-solid$ node tools/codebrain.mjs tree src

the cat command already creates the file for you run that codebase file in your root project folder too : maddi/~/proximity-profiles-solid$ 


=== 🧠 CODEBRAIN ARCHITECTURE ANALYSIS ===
Project: proximity-profiles-solid
Files Analyzed: 60 | Depth: unlimited

📂 DIRECTORY STRUCTURE WITH CODE REFERENCES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

src/
├── 🎯 Entry Points (2)
│   ├── App.jsx
│   │   📄 src/App.jsx
│   │   ├─ Imports: @solidjs/router, solid-js, MainLayout, SheetLayout
│   │   └─ Functions: App
│
│   ├── main.jsx
│   │   📄 src/main.jsx
│   │   ├─ Imports: solid-js/web, App
│
├── 📱 Features (8)
│   ├── dynamicIsland/ (8 files)
│   │
│   ├── 🧩 Components (5)
│   │   ├── BalanceWarning.jsx
│   │   │   📄 src/features/dynamicIsland/components/BalanceWarning.jsx
│   │   │   ├─ Imports: solid-js, proximityStore, island.module
│   │   │   └─ Key Function: BalanceWarning() - 21 lines
│   │   ├── DynamicIsland.jsx
│   │   │   📄 src/features/dynamicIsland/components/DynamicIsland.jsx
│   │   │   ├─ Imports: solid-js, islandStore, notificationStore...
│   │   │   └─ Key Function: DynamicIsland() - 60 lines
│   │   ├── CompactMode.jsx
│   │   │   📄 src/features/dynamicIsland/components/modes/CompactMode.jsx
│   │   │   ├─ Imports: island.module
│   │   │   └─ Key Function: CompactMode() - 14 lines
│   │   ├── NotificationMode.jsx
│   │   │   📄 src/features/dynamicIsland/components/modes/NotificationMode.jsx
│   │   │   ├─ Imports: NotificationView, solid-js, island.module
│   │   │   └─ Key Function: NotificationMode() - 22 lines
│   │   └── ProximityMode.jsx
│   │       📄 src/features/dynamicIsland/components/modes/ProximityMode.jsx
│   │       ├─ Imports: ProximityList, island.module
│   │       └─ Key Function: ProximityMode() - 28 lines
│   │
│   ├── 💾 Stores (1)
│   │   └── islandStore.js
│   │       📄 src/features/dynamicIsland/store/islandStore.js
│   │       └─ Used by: 1 file
│   │           - DynamicIsland.jsx
│
│   ├── errors/ (3 files)
│   │
│   └── 🛠️ Utils (1)
│       └── errorHandler.js
│           📄 src/features/errors/utils/errorHandler.js
│           ├─ Exports: handleError
│
│   ├── loading/ (5 files)
│   │
│   ├── 🧩 Components (2)
│   │   ├── LoadingButton.jsx
│   │   │   📄 src/features/loading/components/LoadingButton.jsx
│   │   │   ├─ Imports: solid-js, LoadingSpinner, loading.module
│   │   │   └─ Key Function: LoadingButton() - 62 lines
│   │   └── LoadingSpinner.jsx
│   │       📄 src/features/loading/components/LoadingSpinner.jsx
│   │       ├─ Imports: loading.module
│   │       └─ Key Function: LoadingSpinner() - 15 lines
│   │
│   ├── 🎣 Hooks (1)
│   │   └── useLoading.js
│   │       📄 src/features/loading/hooks/useLoading.js
│   │       ├─ Exports: useLoading()
│   │       └─ Used by: useProfileActions.js
│   │
│   ├── 💾 Stores (1)
│   │   └── loadingStore.js
│   │       📄 src/features/loading/store/loadingStore.js
│   │       └─ Used by: 1 file
│   │           - useLoading.js
│
│   ├── menu/ (1 files)
│   │
│   ├── 🧩 Components (1)
│   │   └── Menu.jsx
│   │       📄 src/features/menu/Menu.jsx
│   │       ├─ Imports: solid-js, @solidjs/router, menu.module
│   │       └─ Key Function: Menu() - 67 lines
│
│   ├── notifications/ (5 files)
│   │
│   ├── 🧩 Components (1)
│   │   └── NotificationView.jsx
│   │       📄 src/features/notifications/components/NotificationView.jsx
│   │       ├─ Imports: solid-js, notifications.module
│   │       └─ Key Function: NotificationView() - 51 lines
│   │
│   ├── 🎣 Hooks (1)
│   │   └── useNotifications.js
│   │       📄 src/features/notifications/hooks/useNotifications.js
│   │       ├─ Exports: useNotifications()
│   │       └─ Used by: useProfileActions.js
│   │
│   ├── 💾 Stores (2)
│   │   ├── activityStore.js
│   │   │   📄 src/features/notifications/store/activityStore.js
│   │   │   └─ Used by: 3 files
│   │   │       - useProfileActions.js
│   │   │       - ActivityHistory.jsx
│   │   │       - UserProfile.jsx
│   │   └── notificationStore.js
│   │       📄 src/features/notifications/store/notificationStore.js
│   │       └─ Used by: 2 files
│   │           - DynamicIsland.jsx
│   │           - useNotifications.js
│
│   ├── profile/ (4 files)
│   │
│   ├── 🧩 Components (3)
│   │   ├── Card.jsx
│   │   │   📄 src/features/profile/components/Card.jsx
│   │   │   ├─ Imports: card.module
│   │   │   └─ Key Function: Card() - 25 lines
│   │   ├── ProfileHeader.jsx
│   │   │   📄 src/features/profile/components/ProfileHeader.jsx
│   │   │   ├─ Imports: solid-js, profileStore, profile.module
│   │   │   └─ Key Function: ProfileHeader() - 77 lines
│   │   └── ProfileStats.jsx
│   │       📄 src/features/profile/components/ProfileStats.jsx
│   │       ├─ Imports: profileStore, profile.module
│   │       └─ Key Function: ProfileStats() - 32 lines
│   │
│   ├── 💾 Stores (1)
│   │   └── profileStore.js
│   │       📄 src/features/profile/store/profileStore.js
│   │       └─ Used by: 3 files
│   │           - ProfileHeader.jsx
│   │           - ProfileStats.jsx
│   │           - UserProfile.jsx
│
│   ├── proximity/ ⭐ CORE FEATURE (20 files)
│   │
│   ├── 🧩 Components (5)
│   │   ├── ProximityMap.jsx
│   │   │   📄 src/features/proximity/ProximityMap.jsx
│   │   │   ├─ Imports: solid-js, AppleWatchGrid, ProfileSheet...
│   │   │   └─ Key Function: ProximityMap() - 39 lines
│   │   ├── AppleWatchGrid.jsx
│   │   │   📄 src/features/proximity/components/AppleWatchGrid.jsx
│   │   │   ├─ Imports: solid-js, appleWatch.module, honeycombLayout...
│   │   │   └─ Key Function: AppleWatchGrid() - 320 lines
│   │   ├── BlurredBackground.jsx
│   │   │   📄 src/features/proximity/components/BlurredBackground.jsx
│   │   │   ├─ Imports: solid-js
│   │   │   └─ Key Function: BlurredBackground() - 89 lines
│   │   ├── ProfileSheet.jsx
│   │   │   📄 src/features/proximity/components/ProfileSheet.jsx
│   │   │   ├─ Imports: solid-js, useProfileActions, BlurredBackground...
│   │   │   └─ Key Function: ProfileSheet() - 152 lines
│   │   └── ProximityList.jsx
│   │       📄 src/features/proximity/components/ProximityList.jsx
│   │       ├─ Imports: proximity.module
│   │       └─ Key Function: ProximityList() - 33 lines
│   │
│   ├── 🎣 Hooks (6)
│   │   ├── useCulling.js
│   │   │   📄 src/features/proximity/components/canvas/useCulling.js
│   │   │   ├─ Exports: useCulling()
│   │   │   └─ Used by: AppleWatchGrid.jsx
│   │   ├── useSnapback.js
│   │   │   📄 src/features/proximity/components/canvas/useSnapback.js
│   │   │   ├─ Exports: useSnapback()
│   │   │   └─ Used by: AppleWatchGrid.jsx
│   │   ├── useProfileClick.js
│   │   │   📄 src/features/proximity/components/interactions/useProfileClick.js
│   │   │   ├─ Exports: useProfileClick()
│   │   │   └─ Used by: AppleWatchGrid.jsx
│   │   ├── useProfileActions.js
│   │   │   📄 src/features/proximity/hooks/useProfileActions.js
│   │   │   ├─ Exports: useProfileActions()
│   │   │   └─ Used by: ProfileSheet.jsx
│   │   ├── useProfileSelection.js
│   │   │   📄 src/features/proximity/hooks/useProfileSelection.js
│   │   │   ├─ Exports: useProfileSelection()
│   │   │   └─ Used by: ProximityMap.jsx
│   │   └── useProximityTracking.js
│   │       📄 src/features/proximity/hooks/useProximityTracking.js
│   │       ├─ Exports: useProximityTracking()
│   │       └─ Used by: DynamicIsland.jsx
│   │
│   ├── 💾 Stores (2)
│   │   ├── proximityHitsStore.js
│   │   │   📄 src/features/proximity/store/proximityHitsStore.js
│   │   │   └─ Used by: 2 files
│   │   │       - DynamicIsland.jsx
│   │   │       - useProximityTracking.js
│   │   └── proximityStore.js ⚠️ HIGH COUPLING
│   │       📄 src/features/proximity/store/proximityStore.js
│   │       └─ Used by: 5 files
│   │           - BalanceWarning.jsx
│   │           - ProximityMap.jsx
│   │           - useProfileActions.js
│   │           - useProfileSelection.js
│   │           - ActivityHistory.jsx
│   │
│   └── 🛠️ Utils (2)
│       ├── extractDominantColor.js
│       │   📄 src/features/proximity/utils/extractDominantColor.js
│       │   ├─ Exports: extractDominantColor
│       │   └─ Used by: ProfileSheet.jsx
│       └── utils.js
│           📄 src/features/proximity/utils.js
│           ├─ Exports: calculateDistance, createHeart
│
│   └── settings/ (3 files)
    │
    ├── 🧩 Components (2)
    │   ├── SettingsSection.jsx
    │   │   📄 src/features/settings/components/SettingsSection.jsx
    │   │   ├─ Imports: settings.module
    │   │   └─ Key Function: SettingsSection() - 26 lines
    │   └── ThemeToggle.jsx
    │       📄 src/features/settings/components/ThemeToggle.jsx
    │       ├─ Imports: settingsStore, settings.module
    │       └─ Key Function: ThemeToggle() - 30 lines
    │
    ├── 💾 Stores (1)
    │   └── settingsStore.js
    │       📄 src/features/settings/store/settingsStore.js
    │       └─ Used by: 2 files
    │           - ThemeToggle.jsx
    │           - Settings.jsx
│
├── 🗺️  Routes (5)
│   ├── ActivityHistory.jsx
│   │   📄 src/routes/ActivityHistory.jsx
│   │   └─ Imports: solid-js, activityStore, proximityStore, mockData...
│   ├── Dashboard.jsx
│   │   📄 src/routes/Dashboard.jsx
│   │   └─ Imports: routes.module
│   ├── Settings.jsx
│   │   📄 src/routes/Settings.jsx
│   │   └─ Imports: settingsStore, ThemeToggle, SettingsSection, Card...
│   ├── UserProfile.jsx
│   │   📄 src/routes/UserProfile.jsx
│   │   └─ Imports: solid-js, profileStore, ProfileHeader, ProfileStats...
│   └── index.jsx
│       📄 src/routes/index.jsx
│
└── 🎨 Layouts (3)
    ├── DashboardLayout.jsx
    │   📄 src/layouts/DashboardLayout.jsx
    │   └─ Key Function: DashboardLayout() - 14 lines
    ├── MainLayout.jsx → ProximityMap
    │   📄 src/layouts/MainLayout.jsx
    │   └─ Key Function: MainLayout() - 29 lines
    └── SheetLayout.jsx → Menu
        📄 src/layouts/SheetLayout.jsx
        └─ Key Function: SheetLayout() - 38 lines

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🔗 DEPENDENCY INSIGHTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

⚠️  HOT SPOTS (High Coupling):
  1. proximityStore.js → 5 imports
  2. mockData.js → 4 imports
  3. profileStore.js → 3 imports
  4. constants.js → 3 imports
  5. activityStore.js → 3 imports

⚠️  CROSS-FEATURE DEPENDENCIES (7):
  dynamicIsland/ → proximity/ (BalanceWarning.jsx imports proximityStore.js)
  dynamicIsland/ → notifications/ (DynamicIsland.jsx imports notificationStore.js)
  proximity/ → dynamicIsland/ (ProfileSheet.jsx imports DynamicIsland.jsx)
  proximity/ → loading/ (ProfileSheet.jsx imports LoadingButton.jsx)
  proximity/ → menu/ (ProfileSheet.jsx imports Menu.jsx)
  proximity/ → notifications/ (useProfileActions.js imports useNotifications.js)
  proximity/ → errors/ (useProfileActions.js imports errors)

✅ WELL-ISOLATED FEATURES:
  - errors/ (no external feature dependencies)
  - loading/ (no external feature dependencies)
  - menu/ (no external feature dependencies)
  - notifications/ (no external feature dependencies)
  - profile/ (no external feature dependencies)
  - settings/ (no external feature dependencies)

📊 FEATURE SIZE:
  proximity            20 files (33%) ██████
  dynamicIsland         8 files (13%) ██
  loading               5 files (8%) █
  notifications         5 files (8%) █
  profile               4 files (7%) █
  errors                3 files (5%) █
  settings              3 files (5%) █
  menu                  1 files (2%)

=== Analysis complete ===

maddi/~/proximity-profiles-solid$
