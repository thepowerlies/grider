# Gridder
## A grid generator

v. 0.1.2


Generates a grid similar to bootstrap with given options like custom breakpoints and names (including display styles like "d-md-block").

To use grid generator, add it to your source files:
```sass
@use "~web-grider/sass/grid" as grid with (
  $breakpoints: (
    sm: (breakpoint: 576px, container: 540px),
    lg: (breakpoint: 1200px, container: 1140px),
    xl: (breakpoint: 1440px, container: 1400px),
    my-xl: (breakpoint: 1920px, container: 1600px)
  )
);

@include grid.generate_grid();
```

**Installation**

```console
npm install web-grider
```

**Configuration**
<table>
    <thead>
    <tr>
        <th>Variable</th>
        <th>Default value</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td><code>$row-name:</code></td>
        <td><code>"row"</code></td>
    </tr>
    <tr>
        <td><code>$column-name:</code></td>
        <td><code>"col"</code></td>
    </tr>
    <tr>
        <td><code>$column-count:</code></td>
        <td><code>12</code></td>
    </tr>
    <tr>
        <td><code>$generate-display:</code></td>
        <td><code>true</code></td>
    </tr>
    <tr>
        <td><code>$generate-containers:</code></td>
        <td><code>true</code></td>
    </tr>
    <tr>
        <td><code>$gutter-width:</code></td>
        <td><code>15px</code></td>
    </tr>
    <tr>
        <td><code>$base-container-size:</code></td>
        <td><code>360px</code></td>
    </tr>
    <tr>
        <td><code>$breakpoints:</code></td>
        <td><pre><code>(
   sm: (breakpoint: 576px, container: 540px),
   md: (breakpoint: 768px, container: 720px),
   lg: (breakpoint: 992px, container: 960px),
   xl: (breakpoint: 1200px, container: 1140px)
)</code></pre></td>
    </tr>
    </tbody>
</table>
