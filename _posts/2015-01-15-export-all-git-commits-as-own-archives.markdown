---
layout: post
title: "Export all git commits as own archives"
summary:
---

    currentdir=`pwd`
    tmpdir="/tmp/`date | shasum | tr -d ' '`"
    mkdir -p $tmpdir
    
    revisions=`git rev-list --all --reverse`
    for rev in $revisions; do
        git archive --format=tar.gz $rev > $tmpdir/$rev.tar.gz
    done
    
    echo Stored archives in $tmpdir
     
