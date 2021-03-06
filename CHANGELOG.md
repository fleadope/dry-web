# 0.4.1 - 2016-07-26

### Changed

- Set a higher minimum Ruby version (>= 2.1.0) to match dry-auto_inject (timriley)

# 0.4.0 - 2016-07-26

### Changed

- Require dry-component 0.4.1 for latest `Dry::Component::Container#injector` features and API (timriley)

# v0.3.1 / 2016-06-22

### Changed

- Added a necessary version spec for the dry-component dependency (timriley)

# v0.3.0 / 2016-06-22

### Added

- Added an `Umbrella` subclass of `Dry::Web::Container`, intended to be a single, top-level wrapper around multiple sub-apps in a dry-web project (timriley)
- Added `Dry::Web::Settings`, designed to work as an app's single, top-level settings object (timriley)
- Added `env` config to `Dry::Web::Container`, moved across from dry-component (timriley)

### Changed

- Renamed `Dry::Web::Cli` to `Dry::Web::Console`, to make room for a real CLI in the future, starting with dry-web-roda (timriley)

# v0.2.0 / 2016-06-12

### Changed

- Extracted Roda support into [dry-web-roda](https://github.com/dry-rb/dry-web-roda) (timriley)
- Removed `Dry::Web::Transaction::Composer`, which was offering no value above direct calls to `Dry.Transaction` (timriley)
- Basic skeleton example removed, since skeletons/app generators will soon be provided elsewhere (timriley)

# v0.1.0 / 2016-04-21

### Changed

– Renamed from rodakase to dry-web
– Dependency management features were extracted into [dry-component](https://github.com/dry-rb/dry-component)
– `Rodakase::View` was extracted into the [dry-view](https://github.com/dry-rb/dry-view) gem

# v0.0.1 / 2015-11-13

Awesome, first release on Friday 13th. Let's be optimistic. This release ships with:

- `Rodakase::Container` API for dependency management and component loading
- `Rodakase::Application` customized `Roda::Application` API for web part
- `Rodakase::Transaction` for composing processing pipelines
- `Rodakase::View` an experimental, helper-less, template-as-data view layer
