# Data-science-Truman
Truman Algorithm

Develop an algorithm or pseudocode that calculates the value of a professional based on the selected features and their corresponding weights. 

Consider the following steps in the algorithm: 
- Mention how to collect and normalize data for each feature. 
- Apply weights to each feature to calculate a weighted score. 
- Aggregate the weighted scores to derive a comprehensive valuation. 
- Normalize the final valuation if needed to ensure comparability across different individuals or organizations.

# Psuedo Code:
## Input Required: List of features
organization_reputation
innovation_level 
educational_qualification 
years_experience
impact_on_projects
skills
leadership_skills 
## Output:
Final Valuation

## Step 1: Initialization
organization_reputation <- 9.0 ( out of 10)
innovation_level <- 0.7 (Out of 1)
educational_qualification <- 3 (Out of 4)
years_experience <- 2 (Out of 30)
impact_on_projects <- 85 ( Out of 100 )
skills <- 16 (Out of 100 )
leadership_skills <- 22 (Out of 100 )

## Step 2: Standardize Features
### Sub-step 2.1:normalize_features( feature_value, max_value, min_value )
#### Sub-step 2.1.1:return (feature_value - min_value) / (max_value - min_value)

### Sub-step 2.2:
normalized_organization_reputation = normalize_features(organization_reputation, 0, 10)
normalized_innovation_level = normalize_features(innovation_level, 0, 1)
normalized_educational_qualification = normalize_features(educational_qualification, 0, 4)
normalized_years_experience = normalize_features(years_experience, 0, 30)  
normalized_impact_on_projects = normalize_features(impact_on_projects, 0, 100)
normalized_skills = normalize_features(skills, 0, 100)
normalized_leadership_skills = normalize_features(leadership_skills, 0, 100)





