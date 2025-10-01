def check_movie_ticket_price(age):

    if 0 <= age <= 11:
        category = "Child"
        price = 8.00
    elif 12 <= age <= 17:
        category = "Teen"
        price = 15.00
    else:  # age >= 18
        category = "Adult"
        price = 20.00

    return category, price


age = 16


category, price = check_movie_ticket_price(age)


print(f"Age: {age}")
print(f"Category: {category}")
print(f"Ticket Price: ${price:.2f}")
