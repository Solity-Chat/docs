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
  - time_sent: string
  
  Encrypt on server / user
  
  message_clean -> message_encrypted_popescu {micro backend local} -> server -> {process} -> send_to_receiver -> 
  encrypted_message -> before_display_decrypt 
  
  Electron -> server -> Electron 
  
dns: ec2-18-219-43-178.us-east-2.compute.amazonaws.com
ip: 18.219.43.178
ssh -i key.pem ubuntu@ec2-18-219-43-178.us-east-2.compute.amazonaws.com

curl --data-urlencode user_name=Costin --data-urlencode user_bio=bang --data-urlencode user_password=parola http://18.219.43.178/create_user




