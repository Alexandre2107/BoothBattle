Here is the translated README file in English:

---

# **BoothBattle - Artillery Game with Pose Detection**

**BoothBattle** is an artillery game where players control tanks and must adjust the angle and power of their shots to defeat opponents. What makes this demo innovative is its integration with **player pose detection**, allowing gameplay control through body movements.

## **Game Features**

- **Pose Control**: Using **TensorFlow.js**, the game detects player movements through a webcam. This enables players to fire projectiles by performing specific gestures (e.g., raising an arm), creating an immersive and dynamic control experience.

- **Physics**: Projectiles move according to physical laws, calculating trajectory and impact, adding a level of challenge and strategy to the game.

- **User Interface**: The game includes real-time statistics on shot distance, angle, and tank status, providing players with key information for strategic decision-making.

## **Technologies Used**

- **TensorFlow.js**: Used for **real-time pose detection**, allowing players to control the game with body gestures. TensorFlow.js provides a high-precision pose model for human body tracking.

- **TypeScript**: The game is developed in **TypeScript**, ensuring more robust and maintainable code. Static typing improves development quality and error detection.

- **Vite**: Used as a bundler, **Vite** optimizes workflow and development experience with live reloading and fast build times. It also enhances game loading and execution performance.

## **Project Structure**

The project is organized into independent modules, each responsible for a specific game functionality, such as:

- `gameState.ts` - Manages game states (players, shots, collisions).
- `player.ts` - Player logic and tank control.
- `arrow.ts` - Projectile management and physics.
- `poseDetection.ts` - Integration of TensorFlow.js for pose detection.
- `drawing.ts` - Rendering of the graphical interface and game elements.
- `geometry.ts` - Geometric calculations for projectile trajectories.

## **Game Instructions**

### **How to Start Shooting Mode:**

1. **Initial Position:**
    - The player must stand upright in front of the webcam, with arms relaxed at their sides.

2. **Activate Shooting Mode:**
    - **Player on the left side of the screen**: Move your **left wrist** toward your **right shoulder**. This gesture activates **shooting mode**.
    - **Player on the right side of the screen**: Move your **right wrist** toward your **left shoulder**. This also activates **shooting mode**.

### **Shooting Controls:**

Once shooting mode is activated, you can adjust the shot direction and power as follows:

- **Aim**: Move your **right arm (or left arm if you are the right-side player)** up or down to adjust the **shooting angle**.

- **Adjust Power**: Shot power is adjusted horizontally by moving the **wrist** closer or farther from the **shoulder** (simulating how a bow is held). The farther the wrist is from the shoulder, the greater the shooting power. After 3 seconds without movement, the projectile will be released.

### **Game Tips:**
- For a more accurate shot, ensure controlled movements and clearly perform the shooting gesture.
- Experiment with different angles and power levels to find the best way to hit your opponent.
- It is important to position the camera at a sufficient distance to capture both players' bodies.

## **Installation**

1. Clone the repository:
    ```bash
    git clone https://github.com/your_username/boothbattle.git
    ```  

2. Install dependencies:
    ```bash
    cd boothbattle
    npm install
    ```  

3. Start the development server:
    ```bash
    npm run dev
    ```  

4. Open the game in your browser at `http://localhost:5173`.

---