With the inclusion of the following gradle dependency:

    testCompile 'org.jetbrains.kotlin:kotlin-stdlib-jdk8:1.2.70'
    
The native Intellij "Build Project" and "Rebuild Project" don't pick up changes to the JUnit test.

Part 1 Steps

> Sync project

> Open Intellij and load project

> Refresh gradle

> From menus: Build -> Rebuild Project

> Right click KotlinDebugTest and run

> Add another System.out.println("say something") line to test

> From the menus: Build -> Rebuild Project

> Right click KotlinDebugTest and run

> BUG: new System.out.println() output doesn't show in test output

Part 2 Steps

> Comment out kotlin dependency in build.gradle

> Repeat above steps starting at "Refresh gradle"

> Observe: System.out.println() output does show up
