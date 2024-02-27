## Setting Up Environments
![1](https://github.com/aitudorm/kafka/assets/77835933/7f8e252f-4099-4914-81c4-ed211de00465)\
![1_Kafka_Connection](https://github.com/aitudorm/kafka/assets/77835933/3835d03a-9c99-4257-890c-3290a562a94d)

## #1 : Creating Kafka Topic Task
![2_Creating_Kafka_topic](https://github.com/aitudorm/kafka/assets/77835933/af23a108-eec0-4c0a-81ff-9fc17a5c1daf)

## #2 : Writing and Reading Kafka Topic Task

- Creating 2 sessions - producer and consumer and checking it
- `$KAFKA_HOME/bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic kafka-tst-01 --from-beginning`
- `$KAFKA_HOME/bin/kafka-console-producer.sh --broker-list localhost:9092 --topic kafka-tst-01`
![3_Reading_and_Writing_for_Kafka_topics](https://github.com/aitudorm/kafka/assets/77835933/3de382fc-e681-46ea-8c1e-b71c60e18c5f)
![3_X_Second_Producer](https://github.com/aitudorm/kafka/assets/77835933/eaa43945-af8a-49a5-9ff2-7335f8e158b1)
- Creating another 2 sessions - a producer and a consumer, 4 in total, and check them. As you see all consumers are receiving the messages/events
![3_Y_Second_Consumer](https://github.com/aitudorm/kafka/assets/77835933/190a6cce-3654-46f6-8fc0-9b642360c851)

- Deletion
![3_Z_Deletion](https://github.com/aitudorm/kafka/assets/77835933/0558b97e-458c-4813-afd8-80df724738fb)

## #3 : USING KAFKA CONNECT TO WRITE TO A DESTINATION FILE TASK
- After setting up a custom file into confFile directory, we have to insert some rows
![4_Insert_a_few_rows](https://github.com/aitudorm/kafka/assets/77835933/41cac0c9-f7ae-4bb0-a985-5da738490e75)
- By creating consumer we can see wroten data in our file
![4_Y_Creating_Consumer](https://github.com/aitudorm/kafka/assets/77835933/48390500-badc-4cc2-88a8-c5632a3ea604)
- Running loop to tail the changes
![4_Z_Loop_and_end](https://github.com/aitudorm/kafka/assets/77835933/b3cc9e8b-9a7e-462e-9b93-c6303f135ebd)
- End of loop script
![4_Z_Z_END_OF_Loop](https://github.com/aitudorm/kafka/assets/77835933/cec8a5e2-9cc6-4365-aa35-79e78e05dc24)

## #4 : USING KAFKA CONNECT TO WRITE TO A DESTINATION FILE TASK
- Listing current consumer groups
![5_a_Listing Kafka consumer groups](https://github.com/aitudorm/kafka/assets/77835933/a87555cf-2350-4031-a18d-450141694111)
- Listing active consumer groups
![5_b_listing_active_current_connectors](https://github.com/aitudorm/kafka/assets/77835933/f6ebbcb1-1f8d-4553-a0b8-ab9531c84267)
- Checking their status
![5_c_Staus](https://github.com/aitudorm/kafka/assets/77835933/5e1ddef6-fa10-4409-87ed-ab8b451e256d)
- Changing their topic name - we need to stop and start to make some changes
![5_d_reset_offset](https://github.com/aitudorm/kafka/assets/77835933/c2e7d92b-248f-4e1e-a80b-649a7014f9fc)
- But in my case, I couldn't delete my initial topic but deleted it in the end of practice

## #6 USING KAFKA TO READ FROM DATABASE
- Running dokcer mysql in the second window
![6_a_connection_to_mysql_docker](https://github.com/aitudorm/kafka/assets/77835933/393a8453-0a1b-44a7-93cb-7c1763a82048)
- Connecting to DB
![6_b_mysql_db_creation_and_insertion](https://github.com/aitudorm/kafka/assets/77835933/70744973-a5c3-48fb-8af5-2db4a8e08e54)
- Insert some rows
![6_z_inserting_data_checking](https://github.com/aitudorm/kafka/assets/77835933/bd561a37-be2a-42e6-a832-8b9d4bc1bc45)
- Verifiyng consumer side
![6_zzz_verify_from_consumer_side](https://github.com/aitudorm/kafka/assets/77835933/f7b9088e-42cd-4d75-a0f8-ee6772fbc477)
- Dropping topics
![6_zzzz_dropping_topics](https://github.com/aitudorm/kafka/assets/77835933/2793ef3c-dde7-42a6-acbc-4cc3aec33102)




  


