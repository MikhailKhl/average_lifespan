def calculate_average_lifespan(lifespans):
    total_days = sum(lifespan for lifespan in lifespans)
    num_birds = len(lifespans)
    average_lifespan = total_days / num_birds
    
    years = int(average_lifespan // 365)
    days = int(average_lifespan % 365)
    
    return years, days

# Пример использования
bird_lifespans = [5.2, 7.8, 3.4, 9.1, 6.7]
average_years, average_days = calculate_average_lifespan(bird_lifespans)
print(f"Средняя продолжительность жизни птиц: {average_years} лет, {average_days} дней")
