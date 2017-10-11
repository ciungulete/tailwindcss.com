---
extends: _layouts.markdown
title: "Grid"
---

# Grid

<div class="subnav">
    <a class="subnav-link" href="#usage">Usage</a>
    <a class="subnav-link" href="#responsive">Responsive</a>
    <a class="subnav-link" href="#customizing">Customizing</a>
</div>

Documentation around things like:

- Using percentage width helpers and a flex container to create columns
- Using flex wrap if you want columns to wrap
- Using negative margin and padding helpers to add gutters
- Using the container class if you really give a shit

Basic grid example:

<div class="bg-light-softer text-medium text-sm mb-6">
    <div class="text-dark-soft p-4 leading-none">.flex.flex-wrap</div>
    <div class="flex flex-wrap">
        <div class="w-full md:w-1/3">
            <div class="text-center py-4 bg-dark-softer text-light">
                .md:w-1/3
            </div>
        </div>
        <div class="w-full md:w-1/3">
            <div class="text-center py-4 bg-dark-soft text-light">
                .md:w-1/3
            </div>
        </div>
        <div class="w-full md:w-1/3">
            <div class="text-center py-4 bg-dark-softer text-light">
                .md:w-1/3
            </div>
        </div>
    </div>
</div>

Columns don't need to fill a row:

<div class="bg-light-softer text-medium text-sm mb-6">
    <div class="text-dark-soft p-4 leading-none">.flex.flex-wrap</div>
    <div class="flex flex-wrap">
        <div class="w-full md:w-1/4">
            <div class="text-center py-4 bg-dark-softer text-light">
                .md:w-1/4
            </div>
        </div>
        <div class="w-full md:w-1/4">
            <div class="text-center py-4 bg-dark-soft text-light">
                .md:w-1/4
            </div>
        </div>
        <div class="w-full md:w-1/4">
            <div class="text-center py-4 bg-dark-softer text-light">
                .md:w-1/4
            </div>
        </div>
    </div>
</div>


Columns can be different widths:

<div class="bg-light-softer text-medium text-sm mb-6">
    <div class="text-dark-soft p-4 leading-none">.flex.flex-wrap</div>
    <div class="flex flex-wrap">
        <div class="w-full md:w-1/4">
            <div class="text-center py-4 bg-dark-softer text-light">
                .md:w-1/4
            </div>
        </div>
        <div class="w-full md:w-1/2">
            <div class="text-center py-4 bg-dark-soft text-light">
                .md:w-1/2
            </div>
        </div>
        <div class="w-full md:w-1/4">
            <div class="text-center py-4 bg-dark-softer text-light">
                .md:w-1/4
            </div>
        </div>
    </div>
</div>


Rows can overflow and wrap:

<div class="bg-light-softer text-medium text-sm mb-6">
    <div class="text-dark-soft p-4 leading-none">.flex.flex-wrap</div>
    <div class="flex flex-wrap">
        <div class="w-full md:w-1/3">
            <div class="text-center py-4 bg-dark-softer text-light">
                .md:w-1/3
            </div>
        </div>
        <div class="w-full md:w-1/3">
            <div class="text-center py-4 bg-dark-soft text-light">
                .md:w-1/3
            </div>
        </div>
        <div class="w-full md:w-1/3">
            <div class="text-center py-4 bg-dark-softer text-light">
                .md:w-1/3
            </div>
        </div>
        <div class="w-full md:w-1/3">
            <div class="text-center py-4 bg-dark-soft text-light">
                .md:w-1/3
            </div>
        </div>
        <div class="w-full md:w-1/3">
            <div class="text-center py-4 bg-dark-softer text-light">
                .md:w-1/3
            </div>
        </div>
    </div>
</div>

Columns can have gutters:

<div class="bg-light-softer text-medium text-sm mb-6">
    <div class="text-dark-soft p-4 leading-none">.flex.flex-wrap.pull-x-4</div>
    <div class="flex flex-wrap pull-x-4">
        <div class="w-full md:w-1/3 px-4">
            <div class="text-center py-4 bg-dark-softer text-light">
                <div>.w-full</div>
                <div>.md:w-1/3</div>
                <div>.px-4</div>
            </div>
        </div>
        <div class="w-full md:w-1/3 px-4">
            <div class="text-center py-4 bg-dark-soft text-light">
                <div>.w-full</div>
                <div>.md:w-1/3</div>
                <div>.px-4</div>
            </div>
        </div>
        <div class="w-full md:w-1/3 px-4">
            <div class="text-center py-4 bg-dark-softer text-light">
                <div>.w-full</div>
                <div>.md:w-1/3</div>
                <div>.px-4</div>
            </div>
        </div>
    </div>
</div>


Column widths can be automatic:

<div class="bg-light-softer text-medium text-sm mb-6">
    <div class="text-dark-soft p-4 leading-none">.flex.flex-wrap</div>
    <div class="flex flex-wrap">
        <div class="w-1/4 md:flex-1 md:w-auto">
            <div class="text-center py-4 bg-dark-softer text-light">
                <div>.w-1/4</div>
                <div>.md:flex-1</div>
                <div>.md:w-auto</div>
            </div>
        </div>
        <div class="w-1/4 md:flex-1 md:w-auto">
            <div class="text-center py-4 bg-dark-soft text-light">
                <div>.w-1/4</div>
                <div>.md:flex-1</div>
                <div>.md:w-auto</div>
            </div>
        </div>
        <div class="w-1/4 md:flex-1 md:w-auto">
            <div class="text-center py-4 bg-dark-softer text-light">
                <div>.w-1/4</div>
                <div>.md:flex-1</div>
                <div>.md:w-auto</div>
            </div>
        </div>
        <div class="w-1/4 md:flex-1 md:w-auto">
            <div class="text-center py-4 bg-dark-soft text-light">
                <div>.w-1/4</div>
                <div>.md:flex-1</div>
                <div>.md:w-auto</div>
            </div>
        </div>
        <div class="w-1/4 md:flex-1 md:w-auto">
            <div class="text-center py-4 bg-dark-softer text-light">
                <div>.w-1/4</div>
                <div>.md:flex-1</div>
                <div>.md:w-auto</div>
            </div>
        </div>
    </div>
</div>

Fixed width columns are still respected even if a smaller screen has auto column widths:

<div class="bg-light-softer text-medium text-sm mb-6">
    <div class="text-dark-soft p-4 leading-none">.flex.flex-wrap</div>
    <div class="flex flex-wrap">
        <div class="flex-fill md:w-1/6 md:flex-none">
            <div class="text-center py-4 bg-dark-softer text-light">
                <div>.flex-fill</div>
                <div>.md:w-1/6</div>
                <div>.md:flex-none</div>
            </div>
        </div>
        <div class="flex-fill md:w-1/6 md:flex-none">
            <div class="text-center py-4 bg-dark-soft text-light">
                <div>.flex-fill</div>
                <div>.md:w-1/6</div>
                <div>.md:flex-none</div>
            </div>
        </div>
        <div class="flex-fill md:w-1/6 md:flex-none">
            <div class="text-center py-4 bg-dark-softer text-light">
                <div>.flex-fill</div>
                <div>.md:w-1/6</div>
                <div>.md:flex-none</div>
            </div>
        </div>
        <div class="flex-fill md:w-1/6 md:flex-none">
            <div class="text-center py-4 bg-dark-soft text-light">
                <div>.flex-fill</div>
                <div>.md:w-1/6</div>
                <div>.md:flex-none</div>
            </div>
        </div>
        <div class="flex-fill md:w-1/6 md:flex-none">
            <div class="text-center py-4 bg-dark-softer text-light">
                <div>.flex-fill</div>
                <div>.md:w-1/6</div>
                <div>.md:flex-none</div>
            </div>
        </div>
    </div>
</div>


Use margin auto utilities to accomplish offsets:

<div class="bg-light-softer text-medium text-sm mb-6">
    <div class="text-dark-soft p-4 leading-none">.flex.flex-wrap</div>
    <div class="flex flex-wrap">
        <div class="w-full md:w-1/3 md:ml-auto">
            <div class="text-center py-4 bg-dark-soft text-light">
                <div>.md:w-1/3</div>
                <div>.md:ml-auto</div>
            </div>
        </div>
        <div class="w-full md:w-1/3 md:mr-auto">
            <div class="text-center py-4 bg-dark-softer text-light">
                <div>.md:w-1/6</div>
                <div>.md:mr-auto</div>
            </div>
        </div>
    </div>
</div>