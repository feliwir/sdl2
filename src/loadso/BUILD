cc_library(
	name = "loadso",
	deps = ["//:SDL2internal"] + select({
		"//:windows": [
			"//src/loadso/windows:windows",
		],
		"//conditions:default": [
			"//src/loadso/dlopen:dlopen",
		],
	}),
	visibility = ["//visibility:public"],
)
