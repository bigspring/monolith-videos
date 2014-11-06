monolith-videos
===============

A plugin for Monolith for video content

## Objectives
* A CPT for videos
* Optional taxonomy (via theme options)
* Custom field for video link
* Index view with grid of videos, with auto-generated featured image
* Single video page with automatically embedded responsive video
* Possibly use the video thumbs embed plugin for the auto generated feat image

## What we need to do

* Create the CPT, Taxonomy and custom field
* Maybe use hooks to inject markup around the while loop and the standard snippet part. IE on the video grid view we will need a row to wrap the while loop and some column spans to wrap the snippet/panel part as by default the loop is just horizontally stacked post snippet parts. Doing it this way would avoid having to tamper with the loop-posts part (which I've done on tigercat)
* We will need to bundle the lite version of ACF (which can be disabled if the main version exists), commit the video CPT and tax code to code, bundle or steal the code from the video-thumbs plugin. Include the autoEmbed plugin.
* On the single video view we will need to inject the autoEmbed video code, again possibly with the use of hooks.
