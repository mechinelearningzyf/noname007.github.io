---
layout: post
title:  copy-tools-in-linux
date:   2021-07-29 15:53:45 +0800
---



rsync -avz root@10.26.27.172:/usr/bin/redis-cli .

./redis-cli

ldd `which redis-cli`

rsync -avz root@10.26.27.172:/lib64/libjemalloc.so.1 .

export LD_LIBRARY_PATH=`pwd`

redis-cli

