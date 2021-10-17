# ahipping charge calculator program
def main():
    #local variables
    weight = float(input('Enter the number of pounds your package weighs: '))
    print('Your package weighs ', weight, ' lbs')


def totalShippingCharge(weight):
    RATE_ONE = 1.1
    RATE_TWO = 2.2
    RATE_THREE = 3.7
    RATE_FOUR = 3.8

    if weight <= 2:
        print("Your shipping charge is $",weight * RATE_ONE,".")
    else:
        if 2 < weight <= 6:
            print("Your shipping charge is $",weight * RATE_TWO,".")
        else:
            if 6 < weight <= 10:
                print("Your shipping charge is $",weight * RATE_THREE,".")
            else:
                if weight > 10:
                    print("Your shipping charge is $",weight * RATE_FOUR,".")
               
    print('Thanks for using the Shipping Charge Calculator, Have a Nice Day!')
    
