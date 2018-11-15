cc_library(
	name = "timer",
	hdrs = glob(["*.h"]),
	srcs = glob(["*.c"]),
	deps = ["//:SDL2internal"] + select({
		"//:windows": [
			"//src/timer/windows:windows",
		],
		"//conditions:default": [
			"//src/timer/unix:unix",
		],
	}),
	visibility = ["//visibility:public"],
)
