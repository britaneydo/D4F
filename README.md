![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

# LoreLeaf

LoreLeaf is a cozy fantasy study room web app built for students and made by students. The goal of the project is to help users stay focused, complete study sessions, and feel rewarded through a shared magical tree that grows as users earn focus points through doing their tasks.

Instead of making productivity feel plain or stressful, LoreLeaf turns studying into a calm, fantasy-inspired experience where users can enter a shared library room, start a focus timer, and contribute to a living tree that grows over time.

---

## Project Theme

LoreLeaf combines:

- Fantasy
- Library / study room atmosphere
- Medieval-inspired cozy visuals
- Focus and productivity
- Shared progress through a magical tree

The main idea is simple:

> Study, earn points, and help the magical tree grow.

---

## What Problem Does LoreLeaf Solve?

Many people struggle with staying focused, managing time, and staying consistent with their responsibilities. Traditional productivity tools can feel boring, strict, or stressful.

LoreLeaf makes focus sessions feel more rewarding by combining a Pomodoro-style timer with visual progression. As users complete focus time, they earn points that contribute to a shared tree inside the room.

This gives users a small but meaningful reason to keep going.

---

## Core Features

### Pomodoro Timer

Users can start a study timer with adjustable session lengths.

Current timer rules:

- Minimum session: 20 minutes
- Maximum session: 180 minutes
- Timer increases/decreases in 5-minute steps
- Points are earned while focusing

Point system:

- +1 point every 5 minutes
- +4 bonus points at every 20-minute mark

Example:

A 45-minute session earns:

- +8 at 20 minutes
- +10 at 30 minutes
- +16 at 40 minutes

Total: 34 points

---

### Shared Magical Tree

The room contains a shared magical tree that grows as users earn focus points.

The tree is stored in Supabase and updates based on total shared points.

### Tree Stages

<div align="center">

| Sprout | Baby Tree | Small Tree | Medium Tree | Large Magical Tree |
|:---:|:---:|:---:|:---:|:---:|
| <img src="cozy-study-room/public/assets/Luminous_tree5.png" width="30"/> | <img src="cozy-study-room/public/assets/Luminous_tree4.png" width="45"/> | <img src="cozy-study-room/public/assets/Luminous_tree3.png" width="50"/> | <img src="cozy-study-room/public/assets/Luminous_tree2.png" width="85"/> | <img src="cozy-study-room/public/assets/Luminous_tree1.png" width="90"/> |
| 0 - 10 pts | 11 - 50 pts | 51 - 150 pts | 151 - 500 pts | 501+ pts |

</div>

As the shared point total increases and reaches the next Tree Stage, the tree visually changes in the study room.

---

### Tree Progress Display

The frontend shows the current tree progress so users can understand how close they are to the next stage by hovering over the tree.

The display shows:

- Current total points
- The next required point goal
- How many points are left until the next tree stage or max points

For example:

```txt
Tree Progress
Points: 36 / 51
15 points until Small Tree
```
