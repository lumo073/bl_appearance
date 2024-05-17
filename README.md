# BL APPEARANCE

## Prerequisites

### bl_bridge
- Requires `bl_bridge` [here](https://github.com/Byte-Labs-Studio/bl_bridge).

## Installation Steps

1. **Download and Add fivem-builders**
   - Download the `fivem-builders` repository from [here](https://github.com/Z3rio/fivem-builders).
   - Replace the contents of the `[builders]` directory with the downloaded files from `fivem-builders`.
     - Relative path: `resources\[cfx-default]\[system]\[builders]`

2. **Install Dependencies and Build**
   - Navigate to the main parent directory of `bl_appearance`.
   - Run the following command to install dependencies and build the project:
     ```bash
     pnpm install && pnpm build
     ```
     - This command will also navigate to the `/src` directory and build the necessary files.

3. **Build the `/web` Directory**
   - Navigate to the `web/` directory:
     ```bash
     cd web/
     ```
   - Install the necessary npm packages and build the project:
     ```bash
     npm install or pnpm i
     npm run build or pnpm build
     ```

4. **Testing on a Browser or In-Game**
   - To test the project in a browser or in-game using the local Vite address:
     - Comment out the normal `ui_page` line in the `fxmanifest.lua` file.
     - Uncomment the development URL for `ui_page`.
   - Run the development server:
     - From the `web/` directory:
       ```bash
       npm run dev
       ```
     - Alternatively, run from the main directory using pnpm (this will also run Vite):
       ```bash
       pnpm dev
       ```
