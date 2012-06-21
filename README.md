espeak-scripty
==============

Turns dialog files into their audio output through espeak, in a recursive manner similar to GNU make.

    usage: espeak-scripty <input> [<output>]

    input can be a dialog file (format described later), or a folder to
    recursively check for dialog files, only updating the output files if the
    dialog file's timestamp is newer than the corresponding output file's. This
    allows for efficient recompilation.

    output should be a folder to create output folders in. If not specified, it
    uses the current working directory. Each dialog file is turned into a
    folder of the same name in the output directory - a file called Hilda.txt
    will generate a folder called Hilda.txt, though it *is* a folder, despite
    the extension. To output all generated lines to your speakers instead of
    your filesystem, use "-" as the output.
