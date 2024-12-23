This project implements the ICSC (Intelligent Configuration Space Coverage) methodology, which optimizes system performance in enterprise IT environments by strategically configuring and refining system configuration variables. ICSC addresses the challenge of limited data coverage in the configuration space by identifying the most impactful regions for additional performance measurements, thereby enhancing modeling accuracy while managing the number of configuration vectors. This approach is crucial in scenarios where collecting more data is costly or difficult, ensuring that the system's performance is accurately modeled without the need for extensive and impractical data collection.

The scripts provided in this project support various key aspects of the ICSC process. They begin by identifying the uncovered parts of the configuration space through calculating the complement set of configurations missing from the original dataset. Domain-specific filtering rules are then applied to refine this complement set, eliminating impractical configurations. The scripts further identify and remove configurations that closely resemble existing ones to retain only the most representative configurations. A clustering algorithm is iteratively applied to compute cluster centers, and points within a specified distance are removed until convergence. These centers represent potential new data points, which are then evaluated to determine if they fill new gaps in the data space, using a greedy selection strategy to maximize diversity. Finally, a measure of coverage is introduced to assess how well the generated configurations span the configuration space, providing a quantitative metric for evaluating the ICSC method's effectiveness.

If you have any questions, feel free to contact me.
