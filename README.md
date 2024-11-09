# Detect-Fake-Tasks-using-CGAN

- **Objective**: Train a Discriminator to differentiate between real and fake data due to mobile crowdsourcing concerns, where fake data affects model performance.<br>
- **Methodology**: Applied AdaBoost and Random Forest on real data, then added synthetic data. A two-level classification was used, where the Discriminator filtered fake data, followed by AdaBoost/Random Forest for classifying real tasks.<br>
- **Results**: Without the Discriminator, fake data reduced accuracies: AdaBoost from 0.92 to 0.575; Random Forest from 0.993 to 0.590. After filtering, accuracies rose again to 0.926 for AdaBoost and 0.993 for Random Forest, restoring near-original performance.
