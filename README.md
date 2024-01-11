# Error Description

When I install the package `@capacitor-community/firebase-crashlytics`, everything is going well but, when I run the command `npx cap sync` I get an error message related to cocoapods:

```
LoadError - dlopen(/Library/Ruby/Gems/2.6.0/gems/ffi-1.15.5/lib/ffi_c.bundle, 0x0009): tried:
'/Library/Ruby/Gems/2.6.0/gems/ffi-1.15.5/lib/ffi_c.bundle' (mach-o file, but is an incompatible architecture
(have 'arm64', need 'x86_64')),
'/System/Volumes/Preboot/Cryptexes/OS/Library/Ruby/Gems/2.6.0/gems/ffi-1.15.5/lib/ffi_c.bundle' (no such file),
'/Library/Ruby/Gems/2.6.0/gems/ffi-1.15.5/lib/ffi_c.bundle' (mach-o file, but is an incompatible architecture
(have 'arm64', need 'x86_64')) - /Library/Ruby/Gems/2.6.0/gems/ffi-1.15.5/lib/ffi_c.bundle
/System/Library/Frameworks/Ruby.framework/Versions/2.6/usr/lib/ruby/2.6.0/rubygems/core_ext/kernel_require.rb:54:in
`require'
/System/Library/Frameworks/Ruby.framework/Versions/2.6/usr/lib/ruby/2.6.0/rubygems/core_ext/kernel_require.rb:54:in
`require'
/Library/Ruby/Gems/2.6.0/gems/ffi-1.15.5/lib/ffi.rb:5:in `rescue in <top (required)>'
/Library/Ruby/Gems/2.6.0/gems/ffi-1.15.5/lib/ffi.rb:2:in `<top (required)>'
/System/Library/Frameworks/Ruby.framework/Versions/2.6/usr/lib/ruby/2.6.0/rubygems/core_ext/kernel_require.rb:54:in
`require'
/System/Library/Frameworks/Ruby.framework/Versions/2.6/usr/lib/ruby/2.6.0/rubygems/core_ext/kernel_require.rb:54:in
`require'
/Library/Ruby/Gems/2.6.0/gems/ethon-0.12.0/lib/ethon.rb:2:in `<top (required)>'
/System/Library/Frameworks/Ruby.framework/Versions/2.6/usr/lib/ruby/2.6.0/rubygems/core_ext/kernel_require.rb:54:in
`require'
/System/Library/Frameworks/Ruby.framework/Versions/2.6/usr/lib/ruby/2.6.0/rubygems/core_ext/kernel_require.rb:54:in
`require'
/Library/Ruby/Gems/2.6.0/gems/typhoeus-1.4.0/lib/typhoeus.rb:2:in `<top (required)>'
/System/Library/Frameworks/Ruby.framework/Versions/2.6/usr/lib/ruby/2.6.0/rubygems/core_ext/kernel_require.rb:54:in
`require'
/System/Library/Frameworks/Ruby.framework/Versions/2.6/usr/lib/ruby/2.6.0/rubygems/core_ext/kernel_require.rb:54:in
`require'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-core-1.14.3/lib/cocoapods-core/cdn_source.rb:440:in
`download_typhoeus_impl_async'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-core-1.14.3/lib/cocoapods-core/cdn_source.rb:372:in
`download_and_save_with_retries_async'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-core-1.14.3/lib/cocoapods-core/cdn_source.rb:365:in
`download_file_async'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-core-1.14.3/lib/cocoapods-core/cdn_source.rb:338:in `download_file'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-core-1.14.3/lib/cocoapods-core/cdn_source.rb:284:in
`ensure_versions_file_loaded'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-core-1.14.3/lib/cocoapods-core/cdn_source.rb:208:in `search'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-core-1.14.3/lib/cocoapods-core/source/aggregate.rb:83:in `block in
search'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-core-1.14.3/lib/cocoapods-core/source/aggregate.rb:83:in `select'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-core-1.14.3/lib/cocoapods-core/source/aggregate.rb:83:in `search'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/resolver.rb:416:in `create_set_from_sources'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/resolver.rb:385:in `find_cached_set'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/resolver.rb:360:in `specifications_for_dependency'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/resolver.rb:165:in `search_for'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/resolver.rb:274:in `block in sort_dependencies'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/resolver.rb:267:in `each'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/resolver.rb:267:in `sort_by'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/resolver.rb:267:in `sort_by!'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/resolver.rb:267:in `sort_dependencies'
/Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/delegates/specification_provider.rb:60:in `block in
sort_dependencies'
/Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/delegates/specification_provider.rb:77:in
`with_no_such_dependency_error_handling'
/Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/delegates/specification_provider.rb:59:in
`sort_dependencies'
/Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolution.rb:754:in `push_state_for_requirements'
/Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolution.rb:744:in
`require_nested_dependencies_for'
/Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolution.rb:727:in `activate_new_spec'
/Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolution.rb:684:in `attempt_to_activate'
/Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolution.rb:254:in `process_topmost_state'
/Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolution.rb:182:in `resolve'
/Library/Ruby/Gems/2.6.0/gems/molinillo-0.8.0/lib/molinillo/resolver.rb:43:in `resolve'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/resolver.rb:94:in `resolve'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/installer/analyzer.rb:1082:in `block in
resolve_dependencies'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/user_interface.rb:64:in `section'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/installer/analyzer.rb:1080:in
`resolve_dependencies'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/installer/analyzer.rb:125:in `analyze'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/installer.rb:422:in `analyze'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/installer.rb:244:in `block in resolve_dependencies'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/user_interface.rb:64:in `section'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/installer.rb:243:in `resolve_dependencies'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/installer.rb:162:in `install!'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/command/install.rb:52:in `run'
/Library/Ruby/Gems/2.6.0/gems/claide-1.0.3/lib/claide/command.rb:334:in `run'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/lib/cocoapods/command.rb:52:in `run'
/Library/Ruby/Gems/2.6.0/gems/cocoapods-1.14.3/bin/pod:55:in `<top (required)>'
/usr/local/bin/pod:23:in `load'
/usr/local/bin/pod:23:in `<main>'
```