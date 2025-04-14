# CodeVideo: Create Software Educational Content in Minutes, Not Hours

![status badge](https://img.shields.io/badge/status-legendary-57D6BB?labelColor=gray)

Create professional, clear, and correct step-by-step software courses, lessons, and tutorials in *minutes*, not days.

Welcome to the CodeVideo framework and ecosystem!

## Highlevel Overview

The following is a listing of packages used around the CodeVideo ecosystem, more or less according to how often they are used:

### Core Layer

[`@fullstackcraftllc/codevideo-types`](https://github.com/codevideo/codevideo-types) - the TypeScript types used around the CodeVideo ecosystem. Used by almost all packages listed further below.

### Virtual Layer (sits on top of core layer)

[`@fullstackcraftllc/codevideo-virtual-ide`](https://github.com/codevideo/codevideo-virtual-ide) - the virtual IDE used for state traversal and reconstitution, comprised of:
  - [`@fullstackcraftllc/codevideo-virtual-file-explorer`](https://github.com/codevideo/codevideo-virtual-file-explorer) - represents the sidebar file explorer in an IDE
  - [`@fullstackcraftllc/codevideo-virtual-editor`](https://github.com/codevideo/codevideo-virtual-editor) - represents a single editor in an IDE
  - [`@fullstackcraftllc/codevideo-virtual-terminal`](https://github.com/codevideo/codevideo-virtual-terminal) - represents a terminal editor in an IDE
  - [`@fullstackcraftllc/codevideo-virtual-author`](https://github.com/codevideo/codevideo-virtual-author) - represents an author that can speak about what is happening in the IDE
  - [`@fullstackcraftllc/codevideo-virtual-mouse`](https://github.com/codevideo/codevideo-virtual-mouse) - represents a mouse that can move to specific locations in the IDE, as well as left and right click

### GUI Layer (sits on top of virtual layer)

- [`@fullstackcraftllc/codevideo-ide-react`](https://github.com/codevideo/codevideo-ide-react) - Currently our only renderer, an advanced React component. This is the component currently used to make the videos. We have plans to build fully SVG and Canvas based editors in the future.

### CLI

[`@fullstackcraftllc/codevideo-cli`](https://github.com/codevideo/codevideo-cli) - the go-based CLI for generating videos from JSON directly on the command line

### Exporters

- [`@fullstackcraftllc/codevideo-exporters`](https://github.com/codevideo/codevideo-exporters) - exports that are 'simpler' and can be run directly in the browser
- [`@fullstackcraftllc/codevideo-advanced-exporters`](https://github.com/codevideo/codevideo-advanced-exporters) - exports that are 'advanced' and require server-side work (fully functional `@fullstackcraftllc/codevideo-ide-react` React component embeds, pandoc for LaTex-based PDF, probably more to come)

### Websites

- [`@fullstackcraftllc/codevideo.io`](https://github.com/codevideo/codevideo.io) [![Netlify Status](https://api.netlify.com/api/v1/badges/a16a5d48-da4e-402e-a3a0-674264823aa0/deploy-status)](https://app.netlify.com/sites/codevideo/deploys) - the CodeVideo homepage
- [`@fullstackcraftllc/studio.codevideo.io`](https://github.com/codevideo/studio.codevideo.io) [![Netlify Status](https://api.netlify.com/api/v1/badges/1ac1a3f0-f67b-4ac9-97d3-7a548dfe209d/deploy-status)](https://app.netlify.com/sites/codevideostudio/deploys) - the CodeVideo Studio
- [`@fullstackcraftllc/docs.codevideo.io`](https://github.com/codevideo/docs.codevideo.io) [![Netlify Status](https://api.netlify.com/api/v1/badges/48e0ddeb-3912-42a2-8275-37cf09d79383/deploy-status)](https://app.netlify.com/sites/docscodevideo/deploys) - the CodeVideo documentation site

### API

- [`@fullstackcraftllc/codevideo-api`](https://github.com/codevideo/codevideo-api) - Our Node Express-based API (however also includes a Go project to manage the puppeteer recording jobs)

### Miscellaneous

- [`@fullstackcraftllc/codevideo-white-paper`](https://github.com/codevideo/codevideo-white-paper) - The CodeVideo white paper.
- [`@fullstackcraftllc/codevideo-dynamic-ast`](https://github.com/codevideo/codevideo-dynamic-ast) - An AST that can check the static validity of a CodeVideo project at any given action step.

