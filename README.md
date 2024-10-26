# Siyuan Widget: KMind

## Quick Start: /Menu->Widget->KMind

## **KMind Plugin Version is now available at Siyuan Plugin Market, feel free to download**

## QQ Group: 130584086

## Online Feedback: [https://txc.qq.com/products/662653]()

### Reminder: This widget requires KMind plugin API support to enable hovering preview of Siyuan blocks.

### Based on the library developed by [@wangling2](https://github.com/wanglin2). If you find the mind map feature useful, consider [donating](https://wanglin2.github.io/mind-map-docs/sponsor.html) to the original library author to support further development.

## Latest Update Log:

### v2.4.2 (October 8, 2024)

Fixes:

- Fixed the bug where non-Siyuan hyperlink types couldn't navigate properly.

### [v2.4.0 (October 5, 2024)](https://siyuannote.site/x/20241005113503-s68860l)

Description:

- Added the ability to directly create KMind documents in the Siyuan document tree. New node right-click to create Siyuan node sub-documents to adapt to MOC workflow.

New Features:

- Now you can directly create KMind documents in the Siyuan document tree. Operation method: Right-click document tree -> Plugin -> KMind -> Create KMind Document (pro).
- Added function to create associated Siyuan documents directly from nodes; Operation method: Select node -> Right-click node -> Click 'Node Sub-document' (pro).

Optimization & Fixes:

- Optimized the handling of Siyuan hyperlinks in KMind, ensuring correct navigation to specified Siyuan blocks within Siyuan across mobile, docker, and PC platforms, avoiding the issue where clicking the hyperlink in docker would launch the PC client.
- Fixed bug where the widget didn't automatically enter Zen mode during the initial render.
- Optimized the display effect of KMind on mobile; currently view-only, editing is available on PC.

Known Issues:

- KMind's source file saving granularity is the entire document, so do not open the same KMind map simultaneously in the same space! This may lead to data overlap issues, including the following dangerous operations:
  - Opening the same map on multiple devices (even simultaneous opening causes conflicts because KMind also stores view data in source files, and once you open and drag to view, the view data updates, causing discrepancies across devices).
  - Splitting the screen horizontally or vertically with the same map.
  - Other situations of simultaneously opening the same map.
- When opening KMind documents from the document tree, if you switch to a second KMind document before the first one finishes loading, the first document will remain unloaded. Simply toggle the first document off and on to resolve (data is safe and won't be lost).
- Due to the reasons mentioned above, mobile currently only has viewing functionality enabled.

### [v2.3.1 (September 29, 2024)](https://ld246.com/article/1727602784074)

Description:

- Optimized the usage of the widget, improved the display effect of the widget and mirror block mask, optimized the display position of the bottom toolbar.

New Features:

- Added a quick penetration mask function for the widget: hold the ctrl key + left-click the node to quickly focus on the node for direct editing.
- Added Zen mode button to the bottom toolbar, making it accessible directly on mobile without calling out the right-click menu.
- Added one-click jump-to-edit function for mirror blocks; click on the top right corner of the mirror block to jump to the source map for editing (pro).

Optimization:

- Improved the display effect of the widget and mirror block mask, now only displaying mask hints when the mouse hovers over.
- Optimized the position of the bottom toolbar, which now dynamically changes position as the sidebar expands, avoiding overlap.

### v2.3.0 (September 21, 2024)

Description:

- Improved the display & usage of the widget when inserted into documents, adapted to dark mode, and synchronized some features and updates from the upstream library.

New Features:

- Added mask: when inserting the widget into a Siyuan document, you need to click to enter KMind, display the operation UI, and start edit mode. When the mouse leaves the widget area, edit mode exits and UI hides to prevent accidental operations & capture of the main page scroll wheel.
- UI interface automatically adapts to Siyuan's dark mode.
- Custom watermark export.

Others:

- Removed some log outputs, optimized performance.

### v2.2.0 (September 17, 2024)

Description:

- Happy Mid-Autumn Festival~ This is the Mid-Autumn Special Edition.

New Features:

- When creating a new mind map, the sidebar operation bar is hidden by default.

### v2.1.0 (September 4, 2024)

Description:

- Refactoring completed, UI style, operation logic, and new features are consistent with the plugin. For detailed refactoring information, please see the KMind plugin description.

New Features:

- Updated the visual style of the icon, entry: Select node -> Icon -> Emoji icon.

Fixes:

- Fixed the bug where theme switching was not possible due to cross-version updates.
- Fixed import issues.
- Added missing font size 14.

### v2.0.0-beta.3 (April 7, 2024)

Description:

- It's now relatively easy to use rainbow branches, optimizing aesthetics.

Fixes:

- Fixed the bug where the node style settings sometimes couldn't update due to cross-version updates.

New Features:

- Added mind map style settings, allowing customization of line style and color. Entry: left function bar of kmind -> mind map style.
- Added rainbow branches (beta).

Others:

- Updated the underlying library -> 0.9.10.

### v2.0.0-beta.2 (March 31, 2024)

Fixes:

- Fixed the bug where exporting to PDF became unavailable due to version updates. Note, if there are too many nodes, the exported PDF might lose some content. If this occurs, please provide feedback.

### v2.0.0-beta.1 (March 9, 2024)

Update Notes:

- Cross-version update of the underlying library, optimized code structure & performance, possibly with unknown bugs, feedback is welcome.

Breaking Update:

- Upgraded the underlying library -> version 0.9.8, due to design updates of connection lines, connection lines from old data will **not display**! However, it also fixed the bug where custom position saving of connection lines failed. Please upgrade with discretion.

New Features:

- Support for adding summaries to some sub-nodes of the same node.
- Added missing font size 14.

Fixes:

- Fixed the bug where node formatting would sometimes be lost.

### v1.5.0 (February 18, 2024)

New Features:

- Added node search function, shortcut: `ctrl+f`, supporting text content search of nodes; Entry: sidebar toolbar -> search outline.

### v1.4.0 (December 5, 2023)

Fixes:

- Fixed the bug where the outline failed when importing external mind map files.

Optimizations:

- Optimized the response speed of node activation, with toolbar buttons responding faster after clicking a node.
- Optimized outline node clicking; now clicking nodes in the outline automatically activates the canvas and expands to the current active node.

### v1.3.1 (October 17, 2023)

Fixes:

- Fixed the error when importing md files.

Optimizations:

- feat(style.css): Optimized Siyuan hyperlink icon function: narrowed selector range to Siyuan blocks to avoid matching hyperlinks generated by plugins.

### v1.3.0

New Features:

- Added mind map mini-map (thumbnail) [#16](https://github.com/suka233/siyuan-Kmind/issues/16).
- Added mind map read-only mode (need to adapt to Siyuan's document read-only status? Join the group for discussion: 130584086).
- Added mind map zoom toolbar, supporting double-clicking the zoom toolbar to reset zoom.

Optimizations:

- Added overlay instructions for file import to avoid misoperations.

### v1.2.0

Changes:

- Breaking Update: Removed node activation style, changed to default support for node Hover effect (mouse hovering over a node highlights the outer frame).

New Features:

- Support for **cross kmind copy-paste nodes**. Now, you can copy a node from the widget version and paste it directly into the plugin version, and vice versa.
- Pasting plain text data directly onto a node will create a new sub-node with the current clipboard data.
- Pasting images directly onto a node will automatically insert the clipboard image into that node.
- Added node format brush feature: Usage method: Click a node A, then click the format brush button in the top operation bar, and click other nodes to apply the style of node A to others. Clicking anywhere other than nodes will automatically exit the format brush function.
- Pasting clipboard text directly into a node will automatically remove styles, leaving only plain text. If you need to retain the style of the copied text, you can paste it into the node editor by clicking the Node button in the top operation bar.
- When collapsing nodes, the expand button will display how many sub-nodes there are.
- Support for endpoint position of connection lines to follow mouse drag changes.
- Default closed double-click canvas reset.

Fixes:

- Fixed the bug caused by ctrl+v on the root node [#7](https://github.com/suka233/siyuan-kmind-plugin/issues/7).

## Historical Update Log [Click to View](https://github.com/suka233/siyuan-Kmind/blob/dev/CHANGELOG.md)

### Known Defects of This Widget:

1. After directly pasting an image into a node, the image might not display the next time you enter the mind map. You need to double-click the node to display it. It's recommended to use the image button in the top operation button bar to add images to nodes.

### Note:

Please do not provide feedback on the underlying library for issues with this widget!!! I cannot see it, and it will disturb the author of the underlying library. Thank you for your cooperation. This widget is made as a personal hobby and may have stability risks, data risks at your own responsibility.

Use Github for quick feedback [Click Here](https://github.com/suka233/siyuan-Kmind/issues).
Use Tencent Questionnaire for quick feedback or donation [Click Here](https://wj.qq.com/s2/12591272/adf1/).

### Features:

1. Rich text nodes with relatively complete functionality. The full functionality of the original author's project [Demo Address](https://wanglin2.github.io/mind-map/#/).

2. This widget is a simplified version (mainly due to lack of time to add all features). If you need the full version, you can experience it in the original author's project.

3. The original project has an electron branch, meaning it can be used across multiple platforms like Siyuan, as long as you keep the mind map data exported by this widget properly saved, it can be imported anywhere.

4. When a hyperlink inserted in a node is a Siyuan block link (e.g., siyuan://xxxx), hold alt + left-click to pop up a hover preview window (requires KMind plugin support, please download the KMind plugin version from the Siyuan Market plugin area).
![kmindguide.gif](img%2Fkmindguide.gif)

5. Text inside nodes can link to different Siyuan blocks, and the Siyuan hyperlink will display Siyuan's icon for easy recognition.
![siyuanURL.gif](img%2FsiyuanURL.gif)

6. The popup editor inside nodes supports limited markdown syntax, the specific support list is as follows:

````
# Headers

**Bold text**

*Italic*

***Bold italic***

~~Strikethrough~~

- Bullet points

1. Numbered lists

[] Checkboxes

[]() Links

> Blockquote

`Inline code block`

```
Fenced Code block
```

--- Horizontal Rule

````

