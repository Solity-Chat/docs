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
  
> SSH key
-----BEGIN RSA PRIVATE KEY-----
MIIEowIBAAKCAQEAgLuus57c1Z0VI0UBVGMaghZw+cmRxxcs6wT0bsX0PbVVuWLrr3qJ4bOQKsDo
zEcYkbutHR2jqNNrDdoERBT88L1sJu7LdrzfPdG1gzrWdlFcJjbdS1gf54TtzG99gZbLRpUOSL5t
VKvQ9P3Mt+976z+OtPU2hIQuWCpaG/K3OppBCubTJL3Sh2/pE2gfrbQpwpJs5uPgy7qC1ZVAagRd
i8BeDOJwS6Ce9elTliv4BE4269WSCZMMmbj120n3QOXr0QMl1i02wCfEdaOKwdV2E1i6pHiSN1W0
94nsaRW1CT1R7P/lzzpMZ0vWWz4tfmVY2W17nDrLWeYUjq43a21CLQIDAQABAoIBAEjYa3Ju+e3S
1qw/lxIGhnCIfGOMoXY0chGHmz23vI7StvCRvmZtA+r47iKTSOiXbprAxaQNKpgVEqYi8XkJG1yr
A7FAPVgyZm0X5wucVtFbFrb1IuJIur0K5nlhuXaEOwD0xcF6KGnaVALeP2LyHIAxVfKmM7RnC8aO
KLFZ9j8tTHP/aEjt8bzC9HiFWx1gqUym/Wif4mJ4dyONzs9okKuxppmLiDpz2IYn7p+CuFPMFkmY
HERYOk8FbamBRArpUysb0Nr2e39W/ALhGI5hO2HNnWLqPtgFNHe0+AbbBEnIRRw5Y9GQ2sgbtb/2
r0eZRypFUuU8ln3YrxdieyOIR80CgYEA1T4Ut0GeAlSk1GhSv+0Ap4C/c2CsEeUSdc7HPspm7Ql3
HVWPXVvanYX7jvSnL59id653fkbkTIEdY14KzUIOyNMf7Yx7hF2Q81S21N245YWgauWFFp2aVDIC
XKwuKv3+dEUi05u+++J9cTSgQklCk505Ql/j1AjxqjlddqYEA/cCgYEAmoup6RQO+NwGIL7QSmyT
PT68iE2OP452x4+aYDbyvXSfbbc/Zt03r3TauyEXfqGmsfQaQW2QgOkjHbJjEeqXVopyo1sZ789N
Vpts9Z+tFPYBKH+TnyZB2KTTpFZ9hycmmjISvDXBS5xnhtVIMeSYDhmfiZOZFBzgeQzUUJin2fsC
gYBWtooCA0LXu8fTQCD2PtAXTTmNF3ChTj91fIJ1PCUimsi/Ov2zfxilGciz1zTtHqkR9fZNeVJ4
8cAbmjBWS1hrvb6sAIZxywKYkIhQg2EepHoZPgAitC//sN5ZBQM5JFQGv95rolfFYdKU6EuK6POT
x0lzfj7NCF4NVIp3JwdW/QKBgQCE0yB3KDwt+rxxjE3siSCK9M6Iv09QpJrFrVBa/R7nYcJcQ7CE
MgDYFbCgQDK3LSvdqhSewxH9GWKK9XRcQ6lKQbeBWp0SFLM9ilu9Rz001LHuIqe3kuPo1NDpX0SH
0khFImAjzneRCp2XrttbtkJRbAhH78kTFjZ/E12u32Tz3QKBgBL1lxFngI9Ea0ZpuI2whEZIdAsr
ck+e7M4JtK6ljnG2AyskhCnLfG8m/nk9r8mVesZeHUbeAxYrDPkNA47Np+G6tlC8SO09kXl70P2I
jBZxg6/jPO9s4FYPlttX5QfuT5oHmyubP80FQ+ZPDrR4i2pxhwjUIgBYq77iHtuXE0u9
-----END RSA PRIVATE KEY-----

dns: ec2-18-217-217-173.us-east-2.compute.amazonaws.com
ip: 18.217.217.173
