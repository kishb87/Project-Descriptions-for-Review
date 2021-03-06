##Project Overview
The Virtual Tourist app downloads and stores images from Flickr. The app allows users to drop pins on a map, as if they were stops on a tour. Users will then be able to download pictures for the location and persist both the pictures, and the association of the pictures with the pin. 

##Why this project?
The project requires to persist a complex model using Core Data, and plist persistence of an array of dictionaries - core skills required of any iOS Developer.

##What will you learn?
* Use NSURLSessions to interact with a public restful API
* Create a user interface that intuitively communicates network activity and download progress 
* Store media on the device file system
Use Core Data for local persistence of an object structure

##Why is this project meaningful to my career?
The project will give you practice with powerful mechanisms for persisting data locally on a device. Storing media and retrieving it later is an essential skill for any iOS developer.

##How do I complete this project?
1. Download a detailed specification from [here](https://github.com/udacity/Project-Descriptions-for-Review/blob/master/iOS/Virtual%20Tourist%20Specification.pdf).
2. If necessary, review <a href="https://www.udacity.com/course/viewer#!/c-ud325-nd/l-3648658724/m-3748298563" target="_blank">iOS Persistence and Core Data</a> for detailed instructions.
3. Create your app!

##Watch Out!
The app should only interact with Core Data objects (contexts, Persons, and Images) on the main thread. That means that any interactions with these objects inside a networking completion handler should be wrapped in `dispatch_async(dispatch_get_main_queue()) {...}`

If a submission crashes then there may be a race condition, caused by accessing Core Data off the main queue. Make sure to check. In these situations you may be seeing a crash that students don't. It can be very device specific.  If you find a Core Data object being accessed off of the main thread then make sure to include that in your comments to the student, and remind them of the `dispatch_async(dispatch_get_main_queue())` technique.

##Evaluation
Your project will be evaluated by a Udacity Code Reviewer according to the rubric below. All criteria must "meet specifications" in order to pass.

![Virtual Tourist Rubric](https://lh3.googleusercontent.com/Go6qEFlHc4uU88chW6ME841U1aPJpV8t4-fjR_je6i6-l0N0KML8Y5fNHW8M244hYDyQzzWHdvCJycIlGV9K=s0#w=2502&h=3060)
