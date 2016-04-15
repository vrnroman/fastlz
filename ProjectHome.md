FastLZ is a lossless data compression library designed for real-time compression and decompression. It favors **speed** over compression ratio. Decompression requires no memory. Decompression algorithm is very simple, and thus **extremely fast**.

Due to its speed, FastLZ is very useful for applications that need to save some space without a sacrifice in performance. In certain cases, using compressed working data blocks (and decompressing them on-the-fly whenever necessary) actually _may improve_ the performance because the program uses less memory space.

FastLZ is implemented in portable C. It should compile on different platforms without problem.

FastLZ is very small and self-contained. To use it, just add one header file and one source file to the application project. Since it is distributed using MIT license, FastLZ can be used in open-source GPL/LGPL-ed applications as well as proprietary applications.

FastLZ is inspired by Herman Vogt's LZV and Marc Lehmann's LZF algorithms.