# vogro-aio
Asynchronous input and output component of vogro. 

Currently, vogro's asynchronous concurrency model relies on `boost/asio`. As we all know, `boost/asio` is compatible with many different platforms. This does not match the original intention of vogro. Vogro was originally designed to be compatible with only Linux platforms for maximum performance. And relying on `boost/asio` makes vogro lack independence. Users must first install the `boost` package to use vogro. As well as the above considerations, vogro needs to have its own asynchronous input and output concurrent model.
