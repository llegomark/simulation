# Enhanced Simulation of Ragnarok Mobile: Eternal Love 3vs3 PVP Tournament

## Introduction

Greetings! I have been working on a Python code to simulate an upcoming Internal 3vs3 PVP tournament in our striking Hellion Guild. This code showcases my Python skills while providing a fun and interactive tournament simulation for Ragnarok Mobile: Eternal Love.

The simulation simulates an exciting round-robin style tournament between teams of three players. I have incorporated random buffs and debuffs based on the players' job rankings and skill levels to make things more interesting. This introduces a level of unpredictability and strategy to the matches. However, it's important to note that this simulation does not consider the players' equipment, stats, skills, or other attributes. It is purely a simulation and does not reflect the actual gameplay mechanics of Ragnarok Mobile: Eternal Love.

Link: https://llego.dev/posts/epic-3vs3-pvp-simulation-ragnarok-mobile-eternal-love-hellion-guild/

## Code Design

To develop this simulation, I have created several classes and functionalities in the Python code:

### 1. Player, Team, and SkillInteractions Classes

I have defined the `Player`, `Team`, and `SkillInteractions` classes to represent individual players, teams, and skill interactions between players.

The `Player` class represents a player with attributes such as their name, job, skill level, and equipment level. Each player is assigned a random skill level based on their job. The `Player` class also includes methods to calculate the base strength of a player and the modified strength considering skill interactions with their opponents.

The `Team` class represents a team consisting of three players. It includes a method to calculate the team's total strength based on its members' combined strength.

The `SkillInteractions` class handles the skill interactions between players. It defines dictionaries for synergy, counter, status effects, combo breakers, buffs, and debuffs. This class's `apply_skill_interactions` method modifies the players' strengths based on the defined skill interactions.

### 2. Additional Features

In the modified version of the code, I have added some additional features to enhance the simulation:

- **Skill Interactions**: I implemented a class called `SkillInteractions` to handle the skill interactions between players. This class defines dictionaries for various skill interactions such as synergy, counter, status effects, combo breakers, buffs, and debuffs. This class's `apply_skill_interactions` method uses the defined skill interactions to modify the players' strengths.

- **Plotter Class**: I added a `Plotter` class to handle plotting functionalities for the tournament results. This class includes methods for plotting the progression of the winning team's score, the top 3 players based on total strength, the performance of jobs in the tournament, the distribution of player strengths, and the individual strength progression of each player.

### 3. Calculation Functions

I have also included several functions to perform calculations and analysis in the code:

- **calculate_mvp**: This function calculates the Most Valuable Player (MVP) based on the average strength of each player.

- **analyze_skill_pair_data**: This function analyzes the skill pair data after each tournament to detect imbalances. It suggests adjustments to synergy bonuses for overpowered skill combinations.

- **force_skill_pair_rematches**: This function occasionally forces rematches of skill pairs that have yet to be seen often to gather more data.

- **analyze_job_performance**: This function analyzes the performance over time to detect jobs needing buffs or nerfs. It suggests adjustments to job multipliers and rankings accordingly.

- **simulate_tournaments_in_advance**: This function simulates multiple tournaments in advance to forecast expected win rates for players, jobs, and skill pairs. It returns the calculated win rates for further adjustments.

### 4. Constants and Configuration

The code includes certain constants and configuration parameters:

- **JOB_RANKINGS**: A dictionary that defines the base skill level for each job.

- **JOB_MULTIPLIERS**: A dictionary that sets the initial job multipliers for balancing job performance.

- **GAUSSIAN_STD**: The standard deviation used in calculating the base strength of players.

- **NUM_BINS**: The number of bins used in plotting the distribution of player strengths.

## Final Thoughts

With these enhancements, the modified code provides an enhanced and more comprehensive simulation of the 3vs3 PVP tournament in Ragnarok Mobile: Eternal Love. Adding the `SkillInteractions` class and the `Plotter` class increases the flexibility and analytical capabilities of the simulation. Adjusting skill levels, job multipliers, and synergy bonuses based on win rates improves the simulation's balance and fairness.

I hope this updated code contributes to the fun and competitive spirit of the upcoming PVP event. See you on the battleground, and may the best team emerge victorious in Ragnarok Mobile: Eternal Love!

Please feel free to reach out if you have any questions or need further assistance.
