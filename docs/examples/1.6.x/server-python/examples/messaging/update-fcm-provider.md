from appwrite.client import Client

client = Client()
client.set_endpoint('https://cloud.appwrite.io/v1') # Your API Endpoint
client.set_project('<YOUR_PROJECT_ID>') # Your project ID
client.set_key('<YOUR_API_KEY>') # Your secret API key

messaging = Messaging(client)

result = messaging.update_fcm_provider(
    provider_id = '<PROVIDER_ID>',
    name = '<NAME>', # optional
    enabled = False, # optional
    service_account_json = {} # optional
)