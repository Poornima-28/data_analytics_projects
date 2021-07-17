
Project Description

A new function is being developed by the virtual telephony service ‘CallMeMaybe’ that gives information to the supervisors about ineffective operators. An operators is considered to be ineffective if they have many missed call or long waiting times in additions to less outgoing calls

Task : Find the ineffective operators based on incoming / outgoing calls and waiting times

Data Description


telecom_dataset_us.csv:
1. user_id — client account ID
2. date — date the statistics were retrieved
3. direction — call direction (out for outgoing, in for incoming)
4. internal — whether the call was internal (between a client's operators)
5. operator_id — operator identifier
6. is_missed_call — whether the call was missed
7. calls_count — number of calls
8. call_duration — call duration (excluding waiting time)
9. total_call_duration — call duration (including waiting time)


telecom_clients_us.csv:
1. user_id
2. tariff_plan — client's current plan
3. date_start — client's registration date
