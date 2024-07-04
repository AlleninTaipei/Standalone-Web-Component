# Standalone Web Component

This project is done by Calude 3.5.

The overall approach of creating a self-contained, interactive visualization in a single HTML file is sometimes referred to as a "standalone web component" or "self-bootstrapping web application".

This combination of techniques allows for a highly portable, easily shareable visualization that can run directly in a web browser without any build steps or server requirements. It's particularly useful for educational purposes, quick prototypes, or when you want to share a working demo with minimal setup required from the recipient.

|Example: neural network|Methods|Description|
|-|-|-|
|Animation|React Hooks (useState and useEffect)|useState: Used to manage the state of the animation (epoch, phase, activeLayer).|
|||useEffect: Used to create an animation loop that updates the state over time.|
||SVG-based animation|SVG (Scalable Vector Graphics): Used to draw the neural network structure. The animation effect is achieved by dynamically changing the attributes of SVG elements (like colors and stroke widths) based on the current state.|
|Packing|Self-contained HTML file|All necessary code (HTML, CSS, and JavaScript) is combined into a single file. This technique is sometimes referred to as a "single-file application" or "self-contained webpage".|
||Inline scripting|The JavaScript code is embedded directly in the HTML file using a `<script>` tag. We used the "text/babel" type to allow for JSX and modern JavaScript features.|
||CDN (Content Delivery Network)|For dependencies: Instead of bundling React and Babel, we loaded them from a CDN using `<script>` tags. This technique is called "CDN linking" or "external script loading".|

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ by [Allen Sun](https://github.com/allenintaipei)
