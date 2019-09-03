# Setup

## Step 1. Blender Installation for MacOS and Ubuntu Linux (Windows instructions pending)
Download Blender 2.79b for your operating system from the official [Blender release](https://download.blender.org/release/Blender2.79/).

For MacOS the default installation path is
 `/Applications/Blender/blender.app/Contents/MacOS/blender`,
 and for Linux it involves extracting a `blender-2.79b-linux-glibc219-x86_64.tar`  which makes the path
 `<path to extracted tarball>/blender-2.79b-linux-glibc219-x86_64/blender`.

Depending on your OS, add the appropriate path in the `data_generation_parameters.json` file under the key `"blender_path"`.

## Step 2. Download `generate_scene_CRIB.blend`
1.  Download the Blender file `generate_scene_CRIB.blend`, a Blender file containing Toys200 that is used for data generation that is available [here](https://iolfcv.github.io/downloads/index.html).
2. Place the downloaded file at `<path_to_repository>/CRIB_data_generation/generate_scene_CRIB.blend`
3. If setup was done correctly, running `python generate_data.py --demo` in `<path_to_repository>/CRIB_data_generation/` should generate a directory `render_data` with data in it.
