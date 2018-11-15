cc_library(
	name = "main",
	deps = ["//:SDL2internal"] + select({
		"//:windows": [
			"//src/main/windows:windows",
		],
		"//conditions:default": [
			"//src/main/dummy:dummy",
		],
	}),
	visibility = ["//visibility:public"],
)
