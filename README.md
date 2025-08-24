# StateLayer

**A simple, web-based tool for rapidly prototyping spatial UI with a React-like framework.**  
Go from idea to interactive 3D prototype in minutes—right in your browser.

🔗 **Live Demo**: [Try it now](https://statelayer.com)

---

## What is StateLayer?

StateLayer is designed for web developers who want to build for the next generation of computing without the massive learning curve. It bridges the gap between **familiar web technologies** and the **complex world of 3D development**.

Forget slow, complicated game engines and expensive hardware. With StateLayer, you can write **simple, declarative code** that feels like React and see your 3D application come to life instantly in our **live simulator**.

---

## Quick Start: Build a Robot 🤖

You don’t need complex 3D modeling to create interesting things.  
Here’s how you can build and animate a simple robot using only StateLayer primitives.

Just paste this code into the editor:

```javascript
// A friendly, waving robot built with StateLayer primitives

// The Head
Sphere({
  diameter: 1.5,
  position: { y: 3 },
  color: "#cccccc", // A nice silver color
});

// The Body
Box({
  size: { width: 2.5, height: 3, depth: 1.5 },
  position: { y: 1 },
  color: "royalblue",
});

// The "Waving" Arm
Box({
  size: { width: 0.5, height: 1.8, depth: 0.5 },
  position: { x: -2, y: 1.5 },
  color: "#cccccc",
  animation: { rotation: { z: 0.015 } } // A simple waving animation
});

// The other arm
Box({
  size: { width: 0.5, height: 1.8, depth: 0.5 },
  position: { x: 2, y: 1.5 },
  color: "#cccccc",
});

// The Floor
Plane({
  size: { width: 20, height: 20 },
  rotation: { x: Math.PI / 2 }, // Rotate the plane flat
  color: "#444444"
});
```
## Available Components (v0.1.0)

Our MVP component set includes the basic building blocks for most scenes:

- `<Sphere>`
- `<Box>`
- `<Cylinder>`
- `<Plane>`

Each component accepts props like:

- `position`
- `rotation`
- `color`
- `size`
- `animation` (simple rotation/translation animations)

---

## Feedback & Issues

This is a brand new project, and your feedback is critical!  

- 🐞 Found a bug?  
- 💡 Have an idea for a new component?  
- 🎨 Want to share what you’ve built?  

Please open an issue on GitHub — we read every single one.  

➡️ [Open an Issue on GitHub](https://github.com/StatelayerHQ/StateLayer/issues)

---

## Roadmap

We’re just getting started! Based on user feedback, here’s what’s coming next:

- **Interactivity**: `onClick` handlers and other events.  
- **More Components**: `<Text3D>`, `<Image3D>`, and `<Model3D>` for custom models.  
- **User Accounts**: Save and share projects in the cloud.  
