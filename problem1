def find_substrings(patient_dna, virus_dna):
    substrings = []
    virus_length = len(virus_dna)
    
    for i in range(len(patient_dna) - virus_length + 1):
        substring = patient_dna[i:i+virus_length]
        mismatch_count = sum(1 for a, b in zip(substring, virus_dna) if a != b)
        
        if mismatch_count <= 1:
            substrings.append(substring)
    
    return substrings
