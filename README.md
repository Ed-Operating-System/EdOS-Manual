# Official Ed Operating-System Manual

### Last Modified: 25/12/25 (International Date Format)
### Copyright 2025 © Averi

---

This document contains the full detail of the Ed Operating System. All knowledge covered here will try to be dumbed down as much as possible for non-programmers/computer scientists to understand, although still said in a way for people with knowledge within this and/or similar fields to not be bored of the explanation methods.

---

## Table of Contents

### Part I. Introduction & Getting Started
**1. Introduction**   
    1.1 What is EdOS?   
    1.2 Design Philosophy   
    1.3 Goals & Non-Goals   
    1.4 Why x86_64?   
    1.5 x86_64 Architecture Primer   

---

## 1. Introduction

### 1.1 What is EdOS?

EdOS (Ed Operating System) is a 64-bit operating system built from **scratch** for the x86_64 architecture. It's designed as both a functional OS and an educational resource for anyone wanting to understand how operating systems work at a fundamental level. This is an in-house project, by **4veri**, which in simpler terms, means every piece of the operating system is made purely by me, Averi.

Unlike other hobby OS projects that rely on a multitude of prebuilt bootloaders or frameworks, EdOS implements everything from the boot sector up, giving complete control & visibility into every layer of the operating system. EdOS's long-term goal is to be later developed to a point where it can be on par with Linux or Windows. As a whole, it's a platform for learning advanced concepts that prioritizes clarity and education over bloatware and excessive features.

### 1.2 Design Philosophy

When designing an operating system, typically you want set rules to follow, so you don't complicate things later on, confuse yourself, or another reason as to why. Ed has simple yet strict rules to follow. One of our major ones is to create have simplicity before features. A working, simple implementation beats a complex, feature-induced broken one. This doesn't mean Ed strives away from features and ideas, more-so we want to get the product out first before giving it excessive use of broken features.

Another major one is our use of transparent systems. Unlike other operating systems, that hide their work behind multiple layers of abstraction, EdOS keeps almost, if not everything visible. Any system behavior should be easily traced back to the code causing it. This is not only done for me to keep a clean code base, but also for others wanting to learn how Ed, or any generalized operating system works.

The Ed Operating System does have multiple rules to follow, like any other operating system or major system. The list of principles that are followed are found in **Appendix A: EdOS Design Principles**.

### 1.3 Goals & Non-Goals

The Ed Operating System has had many weeks of planning for it's design, architecture, and even future plans for its goals & non-goals. Ed has many goals in mind, such as being bootable on real x86_64 hardware. EdOS is being tested and programmed in a way that allows real hardware to launch our operating system. Another one of our, already explained goals, is making everything in-house, with every system/component, being made my me and potential contributers. As of right now (25/12/25 IDF¹) Ed is in its toddler stages, with a mini-bootloader and no kernel. Even though with what we have at the minute, we hope to have a fully functional, working operating system that's on par with Linux/Windows.

With things you want to happen, you also don't want to happen, EdOS also has many things it doesn't want for its goals, a non-goal. One of Ed's biggest non-goals is POSIX-Complaint. Ed strives to be its own independent piece of technology, that is separate from the rest, while still being talked to at levels of others. Another major one is excessive features; Windows is a major example of having large applications on install. EdOS does want to give *some* form of pre-installed applications, as in clocks, mini-tetris clone, etc, but nothing worth lowering the disk space absurdly.

---

# Appendices

## Appendix A: EdOS Design Principles

This section lists all design principles Ed follows, varying from code structure, to architecture, etc, as this document gets developed, this and other appendices will get reworked, have new stuff written, etc.

- Transparency over abstraction   
- Simplicity before features   
-  Document the struggles, not just the successes   
- Minimal dependencies on external libraries   
- Test on real hardware, not just emulators   
- Performance optimizations require benchmarks   

# Index

IDF¹ - Internation Date Format (YY/MM/DD >> Year/Month/Day)
