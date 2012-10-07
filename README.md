FlurryAnalytics
===============

Integration
1. In the finder, drag FlurryAnalytics/ into project's file folder. (NOTE: If you are upgrading the Flurry iOS SDK, be sure to remove any existing Flurry library folders from your project's file folder before proceeding.)
2. Now add it to your project:
File > Add Files to “Your Project” ... > FlurryAnalytics
-­‐ Destination: select Copy items into destination group’s folder (if needed) -­‐ Folders: Choose 'Create groups for any added folders'
-­‐ Add to targets: select all targets that the lib will be used for
3. In your Application Delegate:
-­‐ Import FlurryAnalytics and inside "applicationDidFinishLaunching:" add: [FlurryAnalytics startSession:@"YOUR_API_KEY"];
#import "FlurryAnalytics.h"
-­‐ (void)applicationDidFinishLaunching:(UIApplication *)application {
[FlurryAnalytics startSession:@"YOUR_API_KEY"];
//your code
}
You're done! That's all you need to do to begin receiving basic metric data.
