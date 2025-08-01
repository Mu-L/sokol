<p align="center">
    <img src="assets/logo_full_large.png" style="width: 60%" /><br/><br/>Simple
    <a href="https://github.com/nothings/stb/blob/master/docs/stb_howto.txt">STB-style</a>
    cross-platform libraries for C and C++, written in C.<br/><br/>
</p>

# Sokol

[**See what's new**](https://github.com/floooh/sokol/blob/master/CHANGELOG.md) (**29-Jun-2025** sokol_imgui.h: updated for Dear ImGui 1.92.0 (some breaking changes!)

[![Build](/../../actions/workflows/main.yml/badge.svg)](/../../actions/workflows/main.yml) [![Bindings](/../../actions/workflows/gen_bindings.yml/badge.svg)](/../../actions/workflows/gen_bindings.yml) [![build](https://github.com/floooh/sokol-zig/actions/workflows/main.yml/badge.svg)](https://github.com/floooh/sokol-zig/actions/workflows/main.yml) [![build](https://github.com/floooh/sokol-nim/actions/workflows/main.yml/badge.svg)](https://github.com/floooh/sokol-nim/actions/workflows/main.yml) [![Odin](https://github.com/floooh/sokol-odin/actions/workflows/main.yml/badge.svg)](https://github.com/floooh/sokol-odin/actions/workflows/main.yml)[![Rust](https://github.com/floooh/sokol-rust/actions/workflows/main.yml/badge.svg)](https://github.com/floooh/sokol-rust/actions/workflows/main.yml)[![Dlang](https://github.com/kassane/sokol-d/actions/workflows/build.yml/badge.svg)](https://github.com/kassane/sokol-d/actions/workflows/build.yml)[![C3](https://github.com/floooh/sokol-c3/actions/workflows/build.yml/badge.svg)](https://github.com/floooh/sokol-c3/actions/workflows/build.yml)

## Examples and Related Projects

- [Live Samples](https://floooh.github.io/sokol-html5/index.html) via WASM ([source](https://github.com/floooh/sokol-samples))

- [Doom Shareware](https://floooh.github.io/doom-sokol/) ported to the Sokol headers ([source](https://github.com/floooh/doom-sokol))

- [Everybody Wants to Crank the World](https://aras-p.github.io/demo-pd-cranktheworld/) demo by
Aras Pranckevičius, PC/web port via sokol ([source](https://github.com/aras-p/demo-pd-cranktheworld)).

- [sokol_gp.h](https://github.com/edubart/sokol_gp) a 2D shape drawing library on top of sokol_gfx.h

- [LearnOpenGL examples ported to sokol-gfx](https://zeromake.github.io/learnopengl-examples/) ([git repo](https://github.com/zeromake/learnopengl-examples))

- [Dear ImGui starterkit](https://github.com/floooh/cimgui-sokol-starterkit) a self-contained starterkit for writing Dear ImGui apps in C.

- [qoiview](https://github.com/floooh/qoiview) a basic viewer for the new QOI image file format

- [Tiny 8-bit emulators](https://floooh.github.io/tiny8bit/)

- A 'single-file' [Pacman clone in C99](https://github.com/floooh/pacman.c/), also available in [Zig](https://github.com/floooh/pacman.zig/)

- [Solar Storm](https://store.steampowered.com/app/2754920/Solar_Storm/), a turn-based scifi artillery game built with Odin and Sokol, released on Steam.

- [Spanking Runners (Samogonki)](https://store.steampowered.com/app/2599800/Spanking_Runners/), arcade racing in a bright and unusual world, released on Steam.

- [MEG-4](https://bztsrc.gitlab.io/meg4) a virtual fantasy console emulator in C89, ported to sokol

- A [Minigolf game](https://mgerdes.github.io/minigolf.html) ([source](https://github.com/mgerdes/minigolf)).

- [hIghQube](https://github.com/RuiVarela/hIghQube) A game demo that used sokol rendering extensively

- [Senos](https://github.com/RuiVarela/Senos) A music app that uses sokol as backend

- ['Dealer's Dungeon'](https://dealers-dungeon.com/demo/) ([lower graphics quality](https://dealers-dungeon.com/demo/?q=3),
[source](https://github.com/bqqbarbhg/spear))

- [Command line tools](https://github.com/floooh/sokol-tools) (shader compiler)

- [How to build without a build system](https://github.com/floooh/sokol-samples#how-to-build-without-a-build-system):
useful details for integrating the Sokol headers into your own project with your favourite C/C++ build system

## Core libraries

- [**sokol\_gfx.h**](https://github.com/floooh/sokol/blob/master/sokol_gfx.h): 3D-API wrapper (GL/GLES3/WebGL2 + Metal + D3D11 + WebGPU)
- [**sokol\_app.h**](https://github.com/floooh/sokol/blob/master/sokol_app.h): app framework wrapper (entry + window + 3D-context + input)
- [**sokol\_time.h**](https://github.com/floooh/sokol/blob/master/sokol_time.h): time measurement
- [**sokol\_audio.h**](https://github.com/floooh/sokol/blob/master/sokol_audio.h): minimal buffer-streaming audio playback
- [**sokol\_fetch.h**](https://github.com/floooh/sokol/blob/master/sokol_fetch.h): asynchronous data streaming from HTTP and local filesystem
- [**sokol\_args.h**](https://github.com/floooh/sokol/blob/master/sokol_args.h): unified cmdline/URL arg parser for web and native apps
- [**sokol\_log.h**](https://github.com/floooh/sokol/blob/master/sokol_log.h): provides a standard logging callback for the other sokol headers

## Utility libraries

- [**sokol\_imgui.h**](https://github.com/floooh/sokol/blob/master/util/sokol_imgui.h): sokol_gfx.h rendering backend for [Dear ImGui](https://github.com/ocornut/imgui)
- [**sokol\_nuklear.h**](https://github.com/floooh/sokol/blob/master/util/sokol_nuklear.h): sokol_gfx.h rendering backend for [Nuklear](https://github.com/Immediate-Mode-UI/Nuklear)
- [**sokol\_gl.h**](https://github.com/floooh/sokol/blob/master/util/sokol_gl.h): OpenGL 1.x style immediate-mode rendering API on top of sokol_gfx.h
- [**sokol\_fontstash.h**](https://github.com/floooh/sokol/blob/master/util/sokol_fontstash.h): sokol_gl.h rendering backend for [fontstash](https://github.com/memononen/fontstash)
- [**sokol\_gfx\_imgui.h**](https://github.com/floooh/sokol/blob/master/util/sokol_gfx_imgui.h): debug-inspection UI for sokol_gfx.h (implemented with Dear ImGui)
- [**sokol\_debugtext.h**](https://github.com/floooh/sokol/blob/master/util/sokol_debugtext.h): a simple text renderer using vintage home computer fonts
- [**sokol\_memtrack.h**](https://github.com/floooh/sokol/blob/master/util/sokol_memtrack.h): easily track memory allocations in sokol headers
- [**sokol\_shape.h**](https://github.com/floooh/sokol/blob/master/util/sokol_shape.h): generate simple shapes and plug them into sokol-gfx resource creation structs
- [**sokol\_color.h**](https://github.com/floooh/sokol/blob/master/util/sokol_color.h): X11 style color constants and functions for creating sg_color objects
- [**sokol\_spine.h**](https://github.com/floooh/sokol/blob/master/util/sokol_spine.h): a sokol-style wrapper around the Spine C runtime (http://en.esotericsoftware.com/spine-in-depth)

## 'Official' Language Bindings

These are automatically updated on changes to the C headers:

- [sokol-zig](https://github.com/floooh/sokol-zig)
- [sokol-odin](https://github.com/floooh/sokol-odin)
- [sokol-nim](https://github.com/floooh/sokol-nim)
- [sokol-rust](https://github.com/floooh/sokol-rust)
- [sokol-d](https://github.com/kassane/sokol-d)
- [sokol-jai](https://github.com/colinbellino/sokol-jai)
- [sokol-c3](https://github.com/floooh/sokol-c3)

## Notes

WebAssembly is a 'first-class citizen', one important motivation for the
Sokol headers is to provide a collection of cross-platform APIs with a
minimal footprint on the web platform while still being useful.

The core headers are standalone and can be used independently from each other.

### Why C:

- easier integration with other languages
- easier integration into other projects
- adds only minimal size overhead to executables

A blog post with more background info: [A Tour of sokol_gfx.h](http://floooh.github.io/2017/07/29/sokol-gfx-tour.html)

# sokol_gfx.h:

- simple, modern wrapper around GLES3/WebGL2, GL3.3, D3D11, Metal, and WebGPU
- buffers, images, shaders, pipeline-state-objects and render-passes
- does *not* handle window creation or 3D API context initialization
- does *not* provide shader dialect cross-translation (**BUT** there's now an 'official' shader-cross-compiler solution which
seamlessly integrates with sokol_gfx.h and IDEs: [see here for details](https://github.com/floooh/sokol-tools/blob/master/docs/sokol-shdc.md)

# sokol_app.h

A minimal cross-platform application-wrapper library:

- unified application entry
- single window or canvas for 3D rendering
- 3D context initialization
- event-based keyboard, mouse and touch input
- supported platforms: Win32, MacOS, Linux (X11), iOS, WASM, Android, UWP
- supported 3D-APIs: GL3.3 (GLX/WGL), Metal, D3D11, GLES3/WebGL2

The vanilla Hello-Triangle using sokol_gfx.h, sokol_app.h and the
sokol-shdc shader compiler (shader code not shown):

```c
#include "sokol_app.h"
#include "sokol_gfx.h"
#include "sokol_log.h"
#include "sokol_glue.h"
#include "triangle-sapp.glsl.h"

static struct {
    sg_pipeline pip;
    sg_bindings bind;
    sg_pass_action pass_action;
} state;

static void init(void) {
    sg_setup(&(sg_desc){
        .environment = sglue_environment(),
        .logger.func = slog_func,
    });

    float vertices[] = {
         0.0f,  0.5f, 0.5f,     1.0f, 0.0f, 0.0f, 1.0f,
         0.5f, -0.5f, 0.5f,     0.0f, 1.0f, 0.0f, 1.0f,
        -0.5f, -0.5f, 0.5f,     0.0f, 0.0f, 1.0f, 1.0f
    };
    state.bind.vertex_buffers[0] = sg_make_buffer(&(sg_buffer_desc){
        .data = SG_RANGE(vertices),
    });

    state.pip = sg_make_pipeline(&(sg_pipeline_desc){
        .shader = sg_make_shader(triangle_shader_desc(sg_query_backend())),
        .layout = {
            .attrs = {
                [ATTR_triangle_position].format = SG_VERTEXFORMAT_FLOAT3,
                [ATTR_triangle_color0].format = SG_VERTEXFORMAT_FLOAT4
            }
        },
    });

    state.pass_action = (sg_pass_action) {
        .colors[0] = { .load_action=SG_LOADACTION_CLEAR, .clear_value={0.0f, 0.0f, 0.0f, 1.0f } }
    };
}

void frame(void) {
    sg_begin_pass(&(sg_pass){ .action = state.pass_action, .swapchain = sglue_swapchain() });
    sg_apply_pipeline(state.pip);
    sg_apply_bindings(&state.bind);
    sg_draw(0, 3, 1);
    sg_end_pass();
    sg_commit();
}

void cleanup(void) {
    sg_shutdown();
}

sapp_desc sokol_main(int argc, char* argv[]) {
    (void)argc; (void)argv;
    return (sapp_desc){
        .init_cb = init,
        .frame_cb = frame,
        .cleanup_cb = cleanup,
        .width = 640,
        .height = 480,
        .window_title = "Triangle",
        .icon.sokol_default = true,
        .logger.func = slog_func,
    };
}
```

# sokol_audio.h

A minimal audio-streaming API:

- you provide a mono- or stereo-stream of 32-bit float samples which sokol_audio.h forwards into platform-specific backends
- two ways to provide the data:
    1. directly fill backend audio buffer from your callback function running in the audio thread
    2. alternatively push small packets of audio data from your main loop,
    or a separate thread created by you
- platform backends:
    - Windows: WASAPI
    - macOS/iOS: CoreAudio
    - Linux: ALSA
    - emscripten: WebAudio + ScriptProcessorNode (doesn't use the emscripten-provided OpenAL or SDL Audio wrappers)

A simple mono square-wave generator using the callback model:

```c
// the sample callback, running in audio thread
static void stream_cb(float* buffer, int num_frames, int num_channels) {
    assert(1 == num_channels);
    static uint32_t count = 0;
    for (int i = 0; i < num_frames; i++) {
        buffer[i] = (count++ & (1<<3)) ? 0.5f : -0.5f;
    }
}

int main() {
    // init sokol-audio with default params
    saudio_setup(&(saudio_desc){
        .stream_cb = stream_cb,
        .logger.func = slog_func,
    });

    // run main loop
    ...

    // shutdown sokol-audio
    saudio_shutdown();
    return 0;
```

The same code using the push-model

```c
#define BUF_SIZE (32)
int main() {
    // init sokol-audio with default params, no callback
    saudio_setup(&(saudio_desc){
        .logger.func = slog_func,
    });
    assert(saudio_channels() == 1);

    // a small intermediate buffer so we don't need to push
    // individual samples, which would be quite inefficient
    float buf[BUF_SIZE];
    int buf_pos = 0;
    uint32_t count = 0;

    // push samples from main loop
    bool done = false;
    while (!done) {
        // generate and push audio samples...
        int num_frames = saudio_expect();
        for (int i = 0; i < num_frames; i++) {
            // simple square wave generator
            buf[buf_pos++] = (count++ & (1<<3)) ? 0.5f : -0.5f;
            if (buf_pos == BUF_SIZE) {
                buf_pos = 0;
                saudio_push(buf, BUF_SIZE);
            }
        }
        // handle other per-frame stuff...
        ...
    }

    // shutdown sokol-audio
    saudio_shutdown();
    return 0;
}
```

# sokol_fetch.h

Load entire files, or stream data asynchronously over HTTP (emscripten/wasm)
or the local filesystem (all native platforms).

Simple C99 example loading a file into a static buffer:

```c
#include "sokol_fetch.h"
#include "sokol_log.h"

static void response_callback(const sfetch_response*);

#define MAX_FILE_SIZE (1024*1024)
static uint8_t buffer[MAX_FILE_SIZE];

// application init
static void init(void) {
    ...
    // setup sokol-fetch with default config:
    sfetch_setup(&(sfetch_desc_t){ .logger.func = slog_func });

    // start loading a file into a statically allocated buffer:
    sfetch_send(&(sfetch_request_t){
        .path = "hello_world.txt",
        .callback = response_callback
        .buffer_ptr = buffer,
        .buffer_size = sizeof(buffer)
    });
}

// per frame...
static void frame(void) {
    ...
    // need to call sfetch_dowork() once per frame to 'turn the gears':
    sfetch_dowork();
    ...
}

// the response callback is where the interesting stuff happens:
static void response_callback(const sfetch_response_t* response) {
    if (response->fetched) {
        // data has been loaded into the provided buffer, do something
        // with the data...
        const void* data = response->buffer_ptr;
        uint64_t data_size = response->fetched_size;
    }
    // the finished flag is set both on success and failure
    if (response->failed) {
        // oops, something went wrong
        switch (response->error_code) {
            SFETCH_ERROR_FILE_NOT_FOUND: ...
            SFETCH_ERROR_BUFFER_TOO_SMALL: ...
            ...
        }
    }
}

// application shutdown
static void shutdown(void) {
    ...
    sfetch_shutdown();
    ...
}
```

# sokol_time.h:

Simple cross-platform time measurement:

```c
#include "sokol_time.h"
...
/* initialize sokol_time */
stm_setup();

/* take start timestamp */
uint64_t start = stm_now();

...some code to measure...

/* compute elapsed time */
uint64_t elapsed = stm_since(start);

/* convert to time units */
double seconds = stm_sec(elapsed);
double milliseconds = stm_ms(elapsed);
double microseconds = stm_us(elapsed);
double nanoseconds = stm_ns(elapsed);

/* difference between 2 time stamps */
uint64_t start = stm_now();
...
uint64_t end = stm_now();
uint64_t elapsed = stm_diff(end, start);

/* compute a 'lap time' (e.g. for fps) */
uint64_t last_time = 0;
while (!done) {
    ...render something...
    double frame_time_ms = stm_ms(stm_laptime(&last_time));
}
```

# sokol_args.h

Unified argument parsing for web and native apps. Uses argc/argv on native
platforms and the URL query string on the web.

Example URL with one arg:

https://floooh.github.io/tiny8bit/kc85.html?type=kc85_4

The same as command line app:

> kc85 type=kc85_4

Parsed like this:

```c
#include "sokol_args.h"

int main(int argc, char* argv[]) {
    sargs_setup(&(sargs_desc){ .argc=argc, .argv=argv });
    if (sargs_exists("type")) {
        if (sargs_equals("type", "kc85_4")) {
            // start as KC85/4
        }
        else if (sargs_equals("type", "kc85_3")) {
            // start as KC85/3
        }
        else {
            // start as KC85/2
        }
    }
    sargs_shutdown();
    return 0;
}
```

See the sokol_args.h header for a more complete documentation, and the [Tiny
Emulators](https://floooh.github.io/tiny8bit/) for more interesting usage examples.
