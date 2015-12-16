# Circular Buffer
This is a circular buffer implementation designed to be used with gigabyte sized buffers. It uses a file as its backing store. The backing file is `mmap`'d into memory. One can lower the resident memory size of the program by advising where the customer cursor is (uses `madvise`). The buffer can be loaded again from the backing file if the program exists. 

Use `godoc` for [documentation](http://godoc.org/github.com/cloudflare/buffer).

For now please check tests for examples.