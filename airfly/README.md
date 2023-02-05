# What's Airfly?

* 產 DAG 自動化
* [airfly github](https://github.com/ryanchao2012/airfly)

# Why airfly?

* 寫 DAG 很煩，寫多了也很無聊，感覺很能自動化，解放 Data Engineer 去做其他更重要的事(例如新的架構)
  * Data Engineer (DAG 管理) + Data Scientist or Data Analyst (商業邏輯開發) 的場景相當常見
    * 商業邏輯的上下游關係， DS/DA 在開發時遠比 DE 清楚的多
    * 如果開發時就能定義好 **上下游**，並且有自動化工具產生 DAG ，那麼就能夠整合到 CI/CD

```python
with xxxx as DAG:
task_1 >> (
    task_2,
    task_3,
    task_4
    ) >>
    task_5
```

# Getting Start

examples : 

1. python operators
   1. simple
   2. complex

2. bash in source code
3. complex in source code



## How it work?

1. BaseTask, TaskPair
2. AirflowDAG

# Integration?

4. 怎麼整合到自己的 Workflow?
5. class variables --> `upstreams`
