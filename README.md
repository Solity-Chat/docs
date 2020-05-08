# Dabatabase model

> User:
  - user_id: Number
  - user_name: String
  - user_bio: String
  - user_is_active: Bool
  - conversations : array
  - friends: array [users]
  - password: string
  
> Conversation
  - conversation_id: Number
  - number_of_messages: Number
  - user_participant1: string
  - user_participant2: string
  - messages: array[message]

> Message
  - message_id: Number
  - message_content: String
  - message_status: Int
  - conversation_id: Number
  - user_id: Int
  - time_sent: string
  
  Encrypt on server / user
  
  message_clean -> message_encrypted_popescu {micro backend local} -> server -> {process} -> send_to_receiver -> 
  encrypted_message -> before_display_decrypt 
  
  Electron -> server -> Electron 
  
dns: ec2-18-219-43-178.us-east-2.compute.amazonaws.com
ip: 18.219.43.178
ssh -i key.pem ubuntu@ec2-18-219-43-178.us-east-2.compute.amazonaws.com

curl --data-urlencode user_name=Costin --data-urlencode user_bio=bang --data-urlencode user_password=parola http://18.219.43.178/create_user

User:
-create an user:
curl --data-urlencode user_name=Costin --data-urlencode user_bio=bang --data-urlencode user_password=parola http://18.219.43.178/create_user

-get user by id:
curl -H "Accept: application/json" http://18.219.43.178/get_user/id_0001

-get user by username:
curl -H "Accept: application/json" http://18.219.43.178/get_user_by_name/Costin

Conversation:
-create a conversation:
curl --data-urlencode user_participant1=Andrei --data-urlencode user_participant2=Costin http://18.219.43.178/create_conversation

-get conversation by id:
curl -H "Accept: application/json" http://18.219.43.178/get_conversation/id_0001

-get conversations by user:
curl -H "Accept: application/json" http://18.219.43.178/get_conversations_by_user/Costin

Message:
-create a message: // la time_sent poti sa pui ce vrei tu
curl --data-urlencode user_id=id_0001 --data-urlencode message_content=Salut --data-urlencode message_status=sent --data-urlencode time_sent=30_04_2020 --data-urlencode conversation_id=id_0002 http://18.219.43.178/create_message

-get message by id:
curl -H "Accept: application/json" http://18.219.43.178/get_message/id_0001

-get messsages by conversation id:
curl -H "Accept: application/json" http://18.219.43.178/get_messages_by_conv/id_0001








