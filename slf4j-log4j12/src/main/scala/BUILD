scala_library(
    sources = ["**/*.scala"],
    compiler_option_sets = ["fatal_warnings"],
    provides = scala_artifact(
        org = "com.twitter",
        name = "twitter-server-slf4j-log4j12",
        repo = artifactory,
    ),
    scope = "forced",  # Exposes a service-loaded class.
    tags = ["logging_impl_check_whitelisted_target"],
    dependencies = [
        "3rdparty/jvm/log4j",
        "3rdparty/jvm/org/slf4j:jcl-over-slf4j",
        "3rdparty/jvm/org/slf4j:jul-to-slf4j",
        "3rdparty/jvm/org/slf4j:slf4j-api",
        "3rdparty/jvm/org/slf4j:slf4j-log4j12",
        "finagle/finagle-base-http/src/main/scala",
        "finagle/finagle-http/src/main/scala",
        "twitter-server/server/src/main/scala",
        "twitter-server/slf4j-log4j12/src/main/resources",
        "util/util-slf4j-api/src/main/scala",
    ],
    exports = [
        "3rdparty/jvm/log4j",
        "3rdparty/jvm/org/slf4j:slf4j-api",
        "3rdparty/jvm/org/slf4j:slf4j-log4j12",
    ],
)
