# ✨ STARLIGHT Protocol

> **A Temporal Traversal-Based Encoding Framework for Educational & Creative Exploration**

---

## 🎯 Overview

**STARLIGHT** is an experimental symbolic encoding protocol that produces cognitively resistant text through an elegant combination of:

- **🔀 Temporal State Mutation** — Weekday-dependent geometric transformations
- **📍 Coordinate-Transfer Mapping** — Position-based symbol reordering
- **⚡ Positional Cyclic Shifts** — Alternating shift patterns for encoding variability
- **🔄 Traversal-Based Reordering** — Lexicographic priority system for word arrangement

Unlike traditional substitution ciphers, STARLIGHT prioritizes **psychological parsing disruption** and **pen-and-paper usability** over computational security.

---

## ⚠️ Disclaimer

**STARLIGHT is an experimental symbolic encoding framework intended for educational, creative, ARG, and protocol-design exploration purposes.**

**It is NOT intended to replace modern cryptographic standards such as AES, RSA, or ChaCha20.**

For production security needs, use battle-tested cryptographic systems. STARLIGHT is for learning, ARGs, puzzles, and creative projects.

---

## 🚀 Quick Start

### Open the Interactive Tool

1. Open `index.html` in your web browser
2. You'll see a 3-column layout:
   - **LEFT:** Base grid editor (7×7 symbol matrix)
   - **CENTER:** Encode/Decode interface with weekday selector
   - **RIGHT:** Protocol visualization + PDF documentation

### Encode a Message

```
1. Enter plaintext in the textarea (e.g., "HELLO WORLD")
2. Select a day (Mon-Sun) for the transformation
3. Click "Encode"
4. See the complete transformation pipeline below
```

### Decode a Message

```
1. Paste the ciphertext + metadata (e.g., "ABC [XYZ]")
2. Select the same day used for encoding
3. Click "Decode"
4. Full decoding trace will display
```

---

## 🎮 Interactive Features

### Base Grid Editor
- **Drag & Drop:** Easily rearrange grid cells by dragging
- **Auto Generate:** Shuffle the grid randomly
- **Validate:** Check for duplicate symbols
- **Reset:** Return to default configuration

### Day-Based Transformations

Each day applies a unique geometric transformation to the 7×7 grid:

| Day | Transformation |
|-----|---|
| **Monday** | Horizontal Mirror |
| **Tuesday** | Vertical Mirror |
| **Wednesday** | Main Diagonal Reflection |
| **Thursday** | Anti-Diagonal Reflection |
| **Friday** | 90° Clockwise Rotation |
| **Saturday** | 90° Counterclockwise Rotation |
| **Sunday** | Center Reflection |

### Protocol Visualization

Below the input panel, watch the **live protocol trace** showing:
- 📊 **Base Grid** — Starting symbol matrix
- 🔄 **Operational Grid** — Transformed matrix for today's day
- 🔤 **Input Tokenization** — How words are split into symbols
- 📍 **Coordinate Remapping** — Base coordinates → Operational coordinates
- ⚡ **Shift Execution** — Positional shift application
- 🔀 **Traversal Word Ordering** — Words sorted by priority
- 🎯 **Final Ciphertext** — Encoded output + metadata

---

## 📋 Symbol Architecture

The STARLIGHT grid contains **49 unique symbols**:

- **26 Letters:** A-Z (priority: Z→A)
- **10 Digits:** 0-9 (priority: 9→0)
- **6 Punctuation:** . , ? ! : ;
- **7 Extended:** MASK, SHF, MIR, ORB, NUL, ECH, SEA

---

## 🔐 Encoding Pipeline

### Step 1: Tokenization
Input words are split into greedy longest-match tokens:
```
"MIRROR" → [MIR, R, O, R]
```

### Step 2: Coordinate Lookup
Find each token's position in the base grid:
```
M @ (0, 0) → Base coordinates found
```

### Step 3: Grid Transformation
Apply day-specific transformation to get operational coordinates:
```
Friday: (r, c) → (c, 6-r)
(0, 0) → (0, 6)
```

### Step 4: Positional Shifting
Apply cyclic shift based on global position:
```
Position 0: No shift
Position 1: +1 shift
Position 2: -1 shift
Pattern: 0, +1, -1, +1, -1...
```

### Step 5: Traversal Ordering
Reorder words by priority (Z→A, 9→0, symbols, punctuation):
```
["ABC", "123", "XYZ"] → ["XYZ", "ABC", "123"]
```

### Step 6: Metadata Encoding
Encode original word positions in Base-48:
```
Position metadata: [0:1:2] → Symbolic representation
```

### Output
```
CIPHERTEXT [METADATA]
```

---

## 🎯 Decoding Pipeline

Reverse the encoding steps:

1. **Extract Metadata** — Parse original word positions
2. **Restore Traversal Order** — Sort back to original order
3. **Reverse Shifts** — Undo positional cyclic shifts
4. **Lookup in Operational Grid** — Find symbols in transformed grid
5. **Transfer to Base Grid** — Get plaintext symbols
6. **Reconstruct Message** — Join tokens back into words

---

## 💻 Technical Stack

- **HTML5** — Structure & semantic markup
- **CSS3** — Portfolio-themed styling with animations
- **JavaScript (ES6+)** — Complete encoding/decoding logic
- **Drag & Drop API** — Interactive grid manipulation

### Browser Support
- Chrome/Chromium 60+
- Firefox 55+
- Safari 10+
- Edge 79+

---

## 🎨 Design Highlights

### Dark Theme
- **Background:** `#0d1117` (GitHub Dark)
- **Primary Accent:** `#58a6ff` (Light Blue)
- **Secondary Accent:** `#79c0ff` (Lighter Blue)
- **Text:** `#d6deea` (Off-White)

### Animations
- Smooth fade-in transitions
- Hover effects on interactive elements
- Grid cell drag feedback
- Modal slide-in animation

### Responsive Layout
- 3-column grid on desktop (1100px+)
- Single column on mobile
- Full-width trace visualization
- Professional monospace typography (JetBrains Mono)

---

## 📚 Files Structure

```
starlight-protocol/
├── README.md           # This file
├── index.html          # Main interactive application
├── STAR_LIGHT.pdf      # Protocol specification document
└── .gitignore          # Git ignore rules
```

---

## 🔗 Links

- **GitHub:** [@Mr-hars007](https://github.com/Mr-hars007)
- **Protocol Paper:** View PDF in app ("Read the Paper Here" button)
- **Live Demo:** [View on GitHub Pages](https://github.com/Mr-hars007/starlight-protocol)

---

## 🎓 Use Cases

### Educational
- Learn about encoding/decoding algorithms
- Understand cryptographic concepts
- Explore grid transformations
- Study symbol manipulation

### Creative
- Design ARG puzzles
- Create encoding challenges
- Build escape room components
- Develop story-based mysteries

### Experimental
- Prototype new protocols
- Explore temporal encoding
- Test psychological parsing disruption
- Research human-operable ciphers

---

## 🛠️ Advanced Features

### Custom Grid Configurations
Modify `defaultGrid` in JavaScript to use custom symbol sets.

### Temporal Variations
The 7-day cycle provides 7 distinct transformation modes. Combine multiple days in sequence for enhanced security.

### Metadata Flexibility
Base-48 encoding allows for large word counts. Supports multi-grid chaining for very long messages.

---

## 📝 Example

**Plaintext:** `HELLO WORLD`

**Day:** Friday (Clockwise Rotation)

**Process:**
1. Tokenize: `[H, E, L, L, O]` `[W, O, R, L, D]`
2. Find coordinates in base grid
3. Transform via Friday rotation
4. Apply shifts: 0, +1, -1, +1, -1
5. Reorder by priority: `WORLD` then `HELLO`
6. Encode metadata: Original positions
7. Output: `[CIPHERTEXT] [METADATA]`

---

## 🚀 Getting Started

1. **Clone the repo:**
   ```bash
   git clone https://github.com/Mr-hars007/starlight-protocol.git
   ```

2. **Open in browser:**
   ```bash
   cd starlight-protocol
   open index.html
   ```

3. **Start encoding!**
   - Type your message
   - Select a day
   - Click Encode/Decode
   - Watch the visualization

---

## 📖 Documentation

Full protocol specification available in `STAR_LIGHT.pdf`:
- Complete mathematical formulation
- All transformation definitions
- Coordinate mapping logic
- Traversal priority system
- Encoding/decoding algorithms

Click **"Read the Paper Here"** in the app to view.

---

## ⭐ Features at a Glance

✅ Interactive 7×7 grid editor  
✅ Drag-and-drop cell rearrangement  
✅ 7 unique weekday transformations  
✅ Real-time protocol visualization  
✅ Complete encoding/decoding traces  
✅ Positional shift demonstrations  
✅ Traversal priority system  
✅ Metadata Base-48 encoding  
✅ Beautiful dark theme  
✅ Responsive design  
✅ PDF documentation viewer  
✅ No dependencies required  

---

## 📄 License

This project is shared for educational, creative, and experimental purposes.

---

## 👨‍💻 Author

**[Mr-hars007](https://github.com/Mr-hars007)** — Protocol Design & Interactive Implementation

---

## 🎯 Protocol Philosophy

> *"STARLIGHT breaks the assumption that all communication must follow natural language parsing. By introducing temporal mutation and position-dependent transformations, we create text that resists both algorithmic and human pattern recognition—not through secret keys, but through deliberate perceptual disruption."*

---

**Disclaimer:** STARLIGHT is an experimental framework for exploration. For production security, use standard cryptographic systems (AES, RSA, ChaCha20). 🔐

---

*Last Updated: May 2026*  
*Protocol Version: 1.0*  
*Interactive Visualizer: Live*

