# 🧠 shared-huffman

**A lightweight Huffman compression algorithm implementation in JavaScript.**  
Effortlessly encode and decode strings using binary trees. Great for learning or integrating into web projects.

<p align="center">
  <a href="https://www.npmjs.com/package/shared-huffman">
    <img src="https://img.shields.io/npm/v/shared-huffman?color=blue&style=flat-square" alt="npm version" />
  </a>
</p>

---

## 🚀 Install

```bash
npm install shared-huffman
```

## 📦 Import

```js
import {
  buildFrequencyMap,
  buildHuffmanTree,
  generateCodes,
  encode,
  decode
} from 'shared-huffman';
```

## 🔍 Example Usage

```js
const str = "hello huffman";

const freqMap = buildFrequencyMap(str);
const tree = buildHuffmanTree(freqMap);
const codeMap = generateCodes(tree);

const encoded = encode(str, codeMap);
console.log("Encoded:", encoded);

const decoded = decode(encoded, tree);
console.log("Decoded:", decoded);
```

## 🧩 Features

- ✅ Simple & Dependency-Free
- ✅ Modern ES Module support
- ✅ Educational use-case for DSA learners
- ✅ Accurate string compression & decompression
- ✅ Plug-and-play for frontend/backend

## 📚 API Reference

- `buildFrequencyMap(str)` → Returns character frequency object
- `buildHuffmanTree(freqMap)` → Builds Huffman tree
- `generateCodes(tree)` → Generates binary codes for each character
- `encode(str, codeMap)` → Encodes a string
- `decode(encodedStr, tree)` → Decodes a binary string

## 📘 Learnings & Why This?

Huffman coding is a fundamental compression technique taught in DSA courses and coding interviews. This project helps you understand:

- ✅ Greedy algorithms in action
- ✅ Binary Trees & Traversals
- ✅ Priority Queues (via frequency sorting)
- ✅ Bitwise compression concepts

## 🌐 Useful Links

- [📦 View on NPM](https://www.npmjs.com/package/shared-huffman)
- [💻 Source on GitHub](https://github.com/mayur777-ui/shared-huffman)

## 👨‍💻 Author

**Mayur Laxkar**  
Full-stack Developer | CS Undergrad  
🌐 [GitHub Profile](https://github.com/mayur777-ui)

## 📄 License

MIT

---

<p align="center">
  ⭐ If you like this project, please give it a star on <a href="https://github.com/mayur777-ui/shared-huffman">GitHub</a>!
</p>
