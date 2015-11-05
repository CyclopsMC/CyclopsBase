## CyclopsBase

This is a simple Cyclops mod template which can be forked when a new mod is started.

### Usage

You will need to fill in the following things when forking this template:

* Move `README_template.md` to `README.md` and fill in the todo's
* Fill in git repo details in `gradle/deploy.gradle`
* Fill in your mod asset location in `gradle/dev.gradle`
* Optionally change versions in `build.properties`
* Update your groupname and archivename in `build.gradle`
* Update secret keys and repo locations in `.travis.yml`
* Rename `Todo.java` and `org.cyclops.todo` for your mod name
* Resolve TODO's in the previously called `Todo.java` class
* Update `MOD_ID`, `MOD_NAME` and `VERSION_URL` in `Reference.java`
* In your `resources/assets`, rename the `todo` to your mod id
* In your `resources`, fill in the mod details in `mcmod.info` and `pack.mcmeta`

If using travis, you will need to enter the following secrets in your build settings:
* `CURSEFORGE_KEY_SECRET`: Your curseforge key for automatic release publishing when a new tag is pushed
* `MAVEN_URL`: (Optional), for automatic dev build publishing
* `MAVEN_USERNAME`: (Optional), maven username for the dev build publishing
* `MAVEN_KEY`: (Optional), maven password for the dev build publishing

### Branching Strategy

For every major Minecraft version, two branches exist:

* `master-{mc_version}`: Latest (potentially unstable) development.
* `release-{mc_version}`: Latest stable release for that Minecraft version. This is also tagged with all mod releases.

### License
All code and images are licenced under the [MIT License](https://github.com/CyclopsMC/CyclopsBase/blob/master-1.8/LICENSE.txt)

