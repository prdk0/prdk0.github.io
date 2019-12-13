---
layout: post
title: "Installtion and Configuration"
date: 2019-12-13
tag: [golang]
comments: true
---
Official binary distributions are available for the FreeBSD (release 10-STABLE and above), Linux, macOS (10.10 and above), and Windows operating systems and the 32-bit (386) and 64-bit (amd64) x86 processor architectures.
<!--more-->

# System requirements

Go [binary distributions](https://golang.org/dl/){:target="\_blank"} are available for these supported operating systems and architectures. Please ensure your system meets these requirements before proceeding. If your OS or architecture is not on the list, you may be able to [install from source](https://golang.org/doc/install/source){:target="\_blank"} or [use gccgo instead](https://golang.org/doc/install/gccgo){:target="\_blank"}.

Download the archive and extract it into /usr/local, creating a Go tree in /usr/local/go. For example:

~~~bash
tar -C /usr/local -xzf go.x.tar.gz
~~~

### snap installation Go

First install __snap__ in to your ubuntu system.
~~~bash
sudo apt install snapd
~~~
__Install Go__
~~~bash
sudo snap install go --classic
~~~

### Setup Go Environment

Add this to your __~/.bashrc__ file

GOROOT is the location where Go package is installed on your system.

~~~bash
export GOROOT=/usr/local/go
~~~

GOPATH is the location of your work directory. For example my project directory is ~/go,
you can create what ever folder structure you want.

~~~bash
export GOPATH=$HOME/go
~~~

Sytem wide PATH setting

~~~bash
export PATH=$GOPATH/bin:$GOROOT/bin:$PATH
~~~

To check the go version installed in your system
~~~bash
go version
~~~
> go version go1.13.5 linux/amd64

Get all go evironment variable settings.

~~~bash
go env
~~~

> 
GOARCH="amd64"
GOBIN=""
GOCACHE="/home/pradeek/.cache/go-build"
GOENV="/home/pradeek/.config/go/env"
GOHOSTARCH="amd64"
GOHOSTOS="linux"
GOOS="linux"
GOPATH="/home/pradeek/go"
GOPROXY="https://proxy.golang.org,direct"
GOROOT="/snap/go/4901"
GOSUMDB="sum.golang.org"
GOTOOLDIR="/snap/go/4901/pkg/tool/linux_amd64"
GCCGO="gccgo"
AR="ar"
CC="gcc"
CXX="g++
....







