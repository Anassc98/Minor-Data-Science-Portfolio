# Training a model

TIjdens het trainen van mijn KNN model, heb ik gebruik gemaakt van een aantal hyperparameters. Op deze manier heb ik geprobeerd om mijn model zo goed mogelijk te trainen. 

## Voorbeeld van mijn hyperparameters:

y= df_userdata['kitchen']
X = df_userdata.drop('kitchen', axis = 1)

y=y.astype('int')

X_main, X_test, y_main, y_test = train_test_split(X, y, test_size = 0.2, random_state=42, stratify=y)
X_train, X_val, y_train, y_val = train_test_split(X_main, y_main, test_size = 0.25, random_state=42, stratify=y_main)
X_test


