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
organization_reputation<br>
innovation_level<br>
educational_qualification<br>
years_experience<br>
impact_on_projects<br>
skills<br>
leadership_skills<br> 
## Output:
Final Valuation

## Step 1: Initialization
organization_reputation <- 9.0 ( out of 10)<br>
innovation_level <- 0.7 (Out of 1)<br>
educational_qualification <- 3 (Out of 4)<br>
years_experience <- 2 (Out of 30)<br>
impact_on_projects <- 85 ( Out of 100 )<br>
skills <- 16 (Out of 100 )<br>
leadership_skills <- 22 (Out of 100 )

## Step 2: Standardize Features
### Sub-step 2.1:
normalize_features( feature_value, max_value, min_value )<br>
#### Sub-step 2.1.1:
return (feature_value - min_value) / (max_value - min_value)<br>

### Sub-step 2.2:
normalized_organization_reputation <- normalize_features(organization_reputation, 0, 10)<br>
normalized_innovation_level <- normalize_features(innovation_level, 0, 1)<br>
normalized_educational_qualification <- normalize_features(educational_qualification, 0, 4)<br>
normalized_years_experience <- normalize_features(years_experience, 0, 30)<br>  
normalized_impact_on_projects <- normalize_features(impact_on_projects, 0, 100)<br>
normalized_skills <- normalize_features(skills, 0, 100)<br>
normalized_leadership_skills <- normalize_features(leadership_skills, 0, 100)<br>

## Step 3: Apply weights to each feature to calculate the weighted score
### Sub-step 3.1: 
Assigned random weights depending on the preference<br>
weight_organization_reputation <- 0.2<br>
weight_innovation_level <- 0.12<br>
weight_educational_qualification <- 0.1<br>
weight_years_experience <- 0.12<br>
weight_impact_on_projects <- 0.15<br>
weight_specialized_skills <- 0.1<br>
weight_leadership_skills <- 0.15<br>

### Sub-step 3.2: Calculate the weighted score<br>
weighted_organization_reputation <- normalized_organization_reputation * weight_organization_reputation<br>
weighted_innovation_level <- normalized_innovation_level * weight_innovation_level<br>
weighted_educational_qualification <- normalized_educational_qualification * weight_educational_qualification<br>
weighted_years_experience <- normalized_years_experience * weight_years_experience<br>
weighted_impact_on_projects <- normalized_impact_on_projects * weight_impact_on_projects<br>
weighted_specialized_skills <- normalized_specialized_skills * weight_specialized_skills<br>
weighted_leadership_skills <- normalized_leadership_skills * weight_leadership_skills<br>

## Step 4: Aggregate the weighted scores to derive a comprehensive valuation
comprehensive_valuation <- (weighted_organization_reputation + weighted_innovation_level +
                           weighted_educational_qualification + weighted_years_experience +
                           weighted_impact_on_projects + weighted_specialized_skills +
                           weighted_leadership_skills)<br>
## Step 5: Normalize the final valuation if needed to ensure comparability across different individuals or organizations
final_valuation <- comprehensive_valuation<br>
print(final_valuation)<br>





