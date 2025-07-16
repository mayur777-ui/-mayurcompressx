# 🧠 shared-huffman

A minimal, blazing-fast JavaScript Huffman Encoder & Decoder – perfect for learning data compression, building educational tools, or adding lightweight compression to your apps.

![npm](https://img.shields.io/npm/v/shared-huffman?color=blue&style=flat-square)
![downloads](https://img.shields.io/npm/dt/shared-huffman?style=flat-square)
![license](https://img.shields.io/npm/l/shared-huffman?style=flat-square)

---

## 📦 Installation

```bash
npm install shared-huffman

---

## 🚀 Use Cases

Here are some real-world and learning-focused use cases where `shared-huffman` shines:

- 🧑‍🎓 **Educational Tools**  
  Perfect for demonstrating how Huffman coding works in computer science or data structure classes.

- ⚙️ **Browser-based Compression**  
  Use it in client-side apps to compress form data, chat messages, or short text before sending.

- 🔍 **Algorithm Visualizers**  
  Integrate with tree-drawing libraries to visualize Huffman trees in real-time.

- 📚 **Competitive Programming / DSA Practice**  
  Great for understanding how frequency-based encoding can optimize storage.

- 🧪 **Testing Compression Concepts**  
  Compare Huffman compression with other techniques like RLE or LZW in small projects.

- 📁 **File-like Encoding**  
  Use it as a starting point for building lightweight, custom file compressors.

---
Code Examples
```js
import {
  buildFrequencyMap,
  buildHuffmanTree,
  generateCodes,
  encode,
  decode
} from 'shared-huffman';

const text = "hello world";

const freqMap = buildFrequencyMap(text);
const tree = buildHuffmanTree(freqMap);
const codeMap = generateCodes(tree);
const compressed = encode(text, codeMap);
const original = decode(compressed, tree);

console.log("Original:", text);
console.log("Compressed:", compressed);
console.log("Decompressed:", original);