# CSEC_CPD
def calculate_minimum_width(n, h, heights):
    total_width = 0
    
    for height in heights:
        if height > h:
            total_width += 2  
        else:
            total_width += 1  
    
    return total_width

if __name__ == "__main__":
    
    n, h = map(int, input().split())     

    heights = list(map(int, input().split()))  

    result = calculate_minimum_width(n, h, heights) 

    print(result)
    
