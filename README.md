# C++ Language and Library Proposals

This repository contains proposals authored and co-authored by @michaelbprice for the ISO/IEC JTC1/SC22/WG21 (ISO C++) programming language.

# Adding a paper

Add a bikeshed source file `.bs` under the `src` directory and be sure to include the following metadata.

```
<pre class='metadata'>
Title: <title-goes-here>
Shortname: <d-or-p-or-n-numbered-paper-without-revision>
Revision: <revision-number-starting-with-zero)>
URL: http://wg21.link/<d-or-p-or-n-numbered-paper-with-revision>
Group: WG21
Audience: <ewg-or-some-other-valid-group>
Status: <D-or-P>
Editor: michael.b.price.dev@gmail.com
Markup Shorthands: markdown yes
No abstract: <true-or-provide-Abstract-metadata>
</pre>
```

Co-authors can be added by adding additional `Editor:` lines to the metadata.

After adding the file in the right location, put the name of the file (without the extension) in the matrix.sources array in `.github/workflows/bikeshed.yaml` for it to be picked up for generation.

# Working in a Codespace

There is a Dev Container specification in this repository that should install the necessary tools if you wish to work within an execution environment.

# Generating Papers

There is a workflow defined in `.github/workflows/bikeshed.yaml` that will run in certain contexts (such as on pushes to a pull request) and will build and validate the papers (as HTML) for submission to WG21.
