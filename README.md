# Rice Cooker CLI

A simple command-line interface (CLI) application for a rice cooker implemented in Kotlin.

## Functionality

1. **Setup Cooking:**
    - Add quantity of rice (can be null).
    - Add quantity of water (can be null).
    - Add temperature (optional, default 100°C).
    - Add timer (optional, default 30 minutes).

2. **Start Cooking:**
    - Will not launch if there is no water.
    - Stops cooking when the timer reaches 0 and launches warm mode.

3. **Warm Mode:**
    - Sets the temperature to 60°C.
    - No timer.

4. **Pause Cooking:**
    - Pauses the timer.
    - Temperature set to 0°C.

5. **Resume Cooking:**
    - Resumes the timer.
    - Temperature set to the value specified in the setup.

## Usage

1. **Setup Cooking:**
    - Enter the quantity of rice (can be null).
    - Enter the quantity of water (can be null).
    - Enter the temperature (optional, default 100°C).
    - Enter the timer (optional, default 30 minutes).

2. **Start Cooking:**
    - Initiates the cooking process.

3. **Warm Mode:**
    - Activated automatically after cooking is complete.

4. **Pause Cooking:**
    - Pauses the cooking process.

5. **Resume Cooking:**
    - Resumes the cooking process.

6. **Check Status:**
    - Displays the current status and temperature.

7. **Quit:**
    - Exits the Rice Cooker CLI.

## How to Run
1. **Download the Project:**

   Clone or download the Kotlin branch of the project from the repository.

   ```bash
   git clone -b feature/kotlin https://github.com/hei-school/cc-d2-my-rice-cooker-miharyjoe.git
   ```

2. Ensure you have Kotlin installed on your machine.
3. Open a terminal and navigate to the directory containing the file.
4. Compile and run the code using the following commands:
   ```bash
   cd cc-d2-my-rice-cooker-miharyjoe
   
   kotlinc MainRiceCooker.kt -include-runtime -d RiceCookerCLI.jar
   
   java -jar RiceCookerCLI.jar
