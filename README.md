# cub3D

## Overview
cub3D is a standout project within the 42 curriculum, designed to provide a hands-on introduction to 3D game development. Inspired by the classic first-person shooter Wolfenstein 3D, it challenges students to build a raycasting-based game engine that renders a 3D environment within a 2D framework.

The project primarily focuses on graphics programming, where you'll need to create a real-time 3D world simulation that the player can navigate through. It's a fantastic opportunity to understand the fundamentals of computer graphics, including raycasting, texture mapping, and creating a dynamic 3D experience.

## Graphics and Controls

*   Smooth Window Management: Ensure smooth window operations, such as changing windows and minimizing.
*   Wall Textures: Display different wall textures based on the wall's orientation (North, South, East, West).
*   Floor and Ceiling Colors: Allow customization of floor and ceiling colors.
*   Controls: Implement intuitive controls, including arrow keys for looking around, WASD for movement, ESC to exit, and window frame's red cross to quit.
*   Image Usage: Strongly recommend using images from miniLibX.

## Map Configuration

*   Scene Description File: Accept a scene description file with a .cub extension as the first argument.
*   Map Constraints: Map Characters: The map must consist of only 6 characters: 0 (empty space), 1 (wall), N, S, E, or W (player's start position and orientation).
*   Map Borders: Ensure the map is surrounded/closed by walls; otherwise, return an error.
*   Map Parsing: Parse the map exactly as it appears in the file, including spaces.
    *   Element Order and Format:
        Each type of element (e.g., textures, colors) can be placed in any order.
    *   Specific information for each element is ordered strictly:
        *   North Texture: NO ./path_to_the_north_texture
        *   South Texture: SO ./path_to_the_south_texture
        *   West Texture: WE ./path_to_the_west_texture
        *   East Texture: EA ./path_to_the_east_texture
        *   Floor Color: F R,G,B (values in range [0,255])
        *   Ceiling Color: C R,G,B (values in range [0,255])

## Error Handling

*   Misconfiguration: If any misconfiguration is detected in the file, the program must exit with "Error\n" followed by an explicit error message.

## Evaluation
#### First submission
11/10/2023  
105%  