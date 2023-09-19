# tflite_flutter_app
using tflite and flutter to code a sign language app

1) create flutter app sample
2) use the main.dart from this code
3) add dependies camera, tflite, tflite helper (can get from the code)
4) flutter pub get
5) add new folder >> assets
6) put in model and labels
7) go to android >> app >> build.gradle
8) change minSdkVersion 23
        targetSdkVersion 33
9) try run without debugging
   : if bug (Build file 'C:\Users\User\AppData\Local\Pub\Cache\hosted\pub.dev\tflite-1.1.2\android\build.gradle' line: 36

* What went wrong:
A problem occurred evaluating project ':tflite'.
> Could not find method compile() for arguments [org.tensorflow:tensorflow-lite:+] on object of type org.gradle.api.internal.artifacts.dsl.dependencies.DefaultDependencyHandler.)
occured
10) the shift + click the path link
11) then go down and changed compile to implementation at
>    dependencies {
        implementation 'org.tensorflow:tensorflow-lite:+'
        implementation 'org.tensorflow:tensorflow-lite-gpu:+'
    }
