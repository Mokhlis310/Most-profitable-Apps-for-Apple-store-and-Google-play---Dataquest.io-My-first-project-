
ages = []
for row in moma:
    date = row[6]
    birth = row[3]
    if birth == '':
        age = 0
        ages.append(age)
    if birth != '':
        age = date - birth
        ages.append(age)
        
final_ages = []
final_age = "Unknown"
for age in ages:
    if age > 20:
        final_ages.append(age)
    else:
        final_ages.append(final_age)
        
    
    
