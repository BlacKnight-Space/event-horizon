# Changelog

## [0.2.0]

### Added

- Timeline now displays an object's events
- Visibility time intervals available for satellites, stations, and notecards; now saved in viewer sessions
- Covariance ellipsoids can be rendered from ephemeris data, with an alpha/opacity slider
- Button to add a facility directly from the lat/lon/alt display
- Option to keep a satellite/station label always pinned/showing
- Preselected color palette added to the color picker
- Remove from viewer option added to the more-actions menu for satellites and stations
- Select all option added to object/station lists
- Moon now rendered in the viewer, toggleable from the top bar, with dynamic lighting
- Save keyboard shortcut, `ctrl+s`
- Confirmation prompt before closing the window with unsaved changes
- Added autosaving viewer sessions to prevent work loss
- Autosave indicator on the session save icon

### Changed

- Standardized time components throughout the UI
- Refreshed styling for station buttons, color/size controls, and the visibility interval editor
- Nicer deletion flow for objects
- Clear screen dialog now matches the app theme
- Reworked animation speed controls, with consistent hover coloring

### Fixed

- Model loading freeze
- Stations and planes not clearing between sessions
- Color slider
- Notecard errors are now caught instead of silently failing
- Notecard size/location no longer vary per monitor
- Non-owners can no longer edit notecards
- Object details button not working in some cases
- Object zoomTo button not working in some cases
- Camera position/zoom not preserved when zoom-to is active
- Objects removed from viewer when deleted
- Description textbox
- Station edit dialog
- Unit step values
- Select-all checkbox no longer shows checked when only partially selected
- Labels no longer disappear at certain zoom levels
- Restart tutorial button
- Datetime picker scaling

## [0.1.2]

### Added

- Scoped swagger docs now available depending on your login state or your pat
- Basic orbital elements plotting introduced (looking for feedback)
- Common name searching for TLE's
- Keyboard shortcuts -> Ctrl+Enter to submit forms, Esc to close panels
- Compact view for session panel
- Satellite Relative Orbits display
- Bulk object creation to streamline workflow
- Removed influxdb and started using timescaledb 

### Changed

- Removed POST `/api/v1/telemetry-data` and replaced with POST `/api/v1/telemetry`
- Removed GET `/api/v1/telemetry-data/:uuid` and replaced with GET `/api/v1/telemetry/:uuid`
- Removed GET `/api/v1/telemetry-data/multiple/:uuids`
- Removed DELETE `/api/v1/telemetry-data/:uuid` and replaced with DELETE `/api/v1/telemetry/:uuid`
- Removed POST `/api/v1/telemetry-data/:uuid/offload` and replaced with POST `/api/v1/telemetry/:uuid/offload`
- Removed GET `/api/v1/health/influxdb`

### Fixed

- If epehemeris file had covariance it was parsed incorrectly
- Adjusted visual consistency for all panels throughout the UI

## [0.1.1]

### Added

- Groups are now supported, making it easier to organize objects.
- New time loop controls let you repeat and review time windows in the viewer.
- Saved sessions now remember your time loop settings.
- Time controls now include helpful tooltips.
- The top bar now shows user account name/details.

### Changed

- The Sessions area has been streamlined to make saving and loading faster and easier.
- Object list and detail views have been refreshed to be cleaner and more compact.

### Fixed

- Fixed toolbar overlap issues so controls no longer block each other.
- Fixed data source connection handling for more reliable TLE updates.
- Fixed ephemeris epoch so shown times match your selected time preference.

### Performance

- Improved startup speed so the viewer loads faster.
- Reduced freezing while loading objects and models.
- Smoother dragging and movement of details panels.
- Improved update timing so motion and display changes feel more responsive.
- General rendering optimizations for better overall performance.

## [0.1.0]

>Initial Release! 🎉
> Welcome to the beta relase of Event Horizon, please submit an issue with any feedback!

### Added

* This changelog!

### Fixed

* None yet, but please submit issues as your find them!
