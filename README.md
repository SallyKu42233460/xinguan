# xinguan
import random

# 假设感染率为 0.1
infection_rate = 0.1

# 假设个人风险因素为 "high" 或 "low"
risk_factor = "high"

# 使用 random.random() 生成 0 到 1 之间的随机数
random_number = random.random()

if risk_factor == "high":
    infection_rate *= 2

# 如果生成的随机数小于感染率，则被感染
if random_number < infection_rate:
    print("You have been infected.")
else:
    print("You have not been infected.")
