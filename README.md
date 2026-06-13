# What is this?
This repository of [nghttp2](https://nghttp2.org/) library header translation for [Free Pascal](https://freepascal.org).

## Building nghttp2 from source code

You will need gcc or clang compiler to build nghttp2 from source code

Clone [nghttp2 git repository](https://github.com/nghttp2/nghttp2)

```
$ git clone git@github.com:nghttp2/nghttp2.git
$ cd nghttp2
$ git submodule update --init
$ autoreconf -i
$ automake
$ autoconf
$ ./configure
$ make 
```
If it is successful then you will have `libs\.libs\libnghttp2.a` file created.

## Usage

Copy `libs\.libs\libnghttp2.a` and `nghttp2.pas` to your Free Pascal project directory.

```
uses nghttp2;
```


