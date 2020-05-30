
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
        
        class NewList(DQ):
    """
    A Python list with some extras!
    """
    def __init__(self, initial_state):
        self.data = initial_state
        self.calc_length()
    
    def append(self, new_item):
        """
        Append `new_item` to the NewList
        """
        self.data = self.data + [new_item]
        self.calc_length()
        
    def calc_length(self):
        length = 0
        for x in self.data:
            length += 1
        self.length = length 
    
