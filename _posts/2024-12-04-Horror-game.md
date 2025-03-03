---
layout: post
title: Making a horror game
date: 2024-11-16 21:01:00
description: My experience making a horror game
tags: Unreal Engine
categories: blender-posts
thumbnail: assets/img/blender/horror.png
---

    <article>
        <header>
            <h1>Challenges in Developing My Horror Game</h1>
            <p><strong>Date:</strong> March 3, 2025 | <strong>Categories:</strong> Game Development</p>
        </header>

        <p>
            Developing my horror game was both an exciting and frustrating journey. While I had a clear vision of the eerie 
            atmosphere and immersive mechanics I wanted to implement, I ran into several challenges along the way. 
            Below are some of the key issues I faced during development and how I approached solving them.
        </p>

        <h2>Issues with Blueprints</h2>
        <p>
            Since I was using Unreal Engine, I initially relied heavily on Blueprints for scripting my gameplay mechanics. 
            While Blueprints are powerful, I quickly found that complex interactions—especially for my rotating puzzle mechanics—became messy.  
            Debugging was difficult as logic chains grew longer, making it hard to track down errors. Eventually, I had to rewrite parts 
            of my system in C++ to gain more control and improve performance.
        </p>

        <h2>Importing Assets</h2>
        <p>
            Asset importing was another major hurdle. Some of the 3D models I downloaded had incorrect scaling, causing objects 
            to appear way too large or too small in my game world. Additionally, texture maps were sometimes broken due to incorrect 
            UV mappings. I had to manually adjust scaling and remap textures in Blender before reimporting them into Unreal Engine.
        </p>

        <h2>Rotating Puzzle Mechanics</h2>
        <p>
            Implementing the rotating puzzles was trickier than expected. I wanted smooth, intuitive controls where players could 
            rotate objects at fixed angles, but Unreal Engine’s default physics sometimes caused jittery movement or unwanted rotations.  
            I experimented with different rotation methods—first using physics constraints, then switching to manually controlled 
            quaternion rotations. In the end, I found that a mix of Timeline nodes in Blueprints with custom logic in C++ gave me the 
            best results.
        </p>

        <h2>Getting Good Lighting</h2>
        <p>
            Horror games rely heavily on atmosphere, and I struggled to get the lighting just right. At first, my game looked too bright 
            and lost its eerie feel. When I reduced the light intensity, some areas became too dark to navigate. I had to balance 
            dynamic lighting with baked lightmaps and tweak post-processing effects like fog, bloom, and ambient occlusion. 
            Additionally, I used subtle flickering lights and shadow-casting objects to enhance the unsettling atmosphere.
        </p>

        <div class="row mt-3">
            <div class="col-sm mt-3 mt-md-0">
                <img src="assets/img/game/horror-lighting.png" alt="Horror Game Lighting" class="img-fluid rounded z-depth-1">
            </div>
        </div>
        
        <div class="caption">
            <p><em>A preview of the game's lighting setup</em></p>
        </div>

        <h2>Final Thoughts</h2>
        <p>
            Despite these challenges, I learned a lot from the development process. Troubleshooting Blueprints, fixing asset imports, 
            refining puzzle mechanics, and optimizing lighting all helped me grow as a game developer. While the game isn't perfect, 
            I'm proud of how it turned out and excited to keep improving it.
        </p>

    </article>

</body>
</html>
