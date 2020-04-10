# Dabatabase model

> User:
  - user_id: Number
  - user_name: String
  - user_bio: String
  - user_is_active: Bool
  
> Conversation
  - conversation_id: Number
  - number_of_messages: Number

> Message
  - user_id_recv: Number
  - user_id_snd: Number
  - message_content: String
  - message_status: Int
  - conversation_id: Number
  
  Encrypt on server / user
  
  message_clean -> message_encrypted_popescu {micro backend local} -> server -> {process} -> send_to_receiver -> 
  encrypted_message -> before_display_decrypt 
  
  Electron -> server -> Electron 
