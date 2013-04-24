Universal-Project-Template-iOS
==============================

Reference project structure for Universal iOS app


Project Structure
-----------------

<ProjectName>.xcodeproj
/<ProjectName>
  /Shared
    /Application      # App delegate and related files
    /Controllers      # Base view controllers
    /Models           # Models, Core Data schema etc
    /Views            # Shared views
    /Library          # Anything that falls outside of the MVC pattern, (e.g. reusable custom views/controls go here)
    /Support          # Categories and helpers
  /iPhone
      ...             # Same structure as 'Shared' but with interface specific classes
  /iPad
      ...
  /Supporting Files   # Prefix headers, main.m, Info.plist
  /Assets             # Images, videos, .strings files
    /Resources        # N/XIBs, Storyboards
    /Images           # Images
  /Vendor             # 3rd party dependencies not managed by CocoaPods
  /Docs
  /Tests
  /Scripts            # All project-related scripts, typically executed as rake tasks using a Rakefile in the project root directory.


References
----------

1. http://www.sebastianrehnby.com/blog/2013/01/15/structuring-an-ios-project/
