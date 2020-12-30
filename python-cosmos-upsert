import os
from azure.cosmos import CosmosClient

connection_string = 'connection_string'
db_name = 'db_name'
container_name = 'container_name'

cosmos_client = CosmosClient.from_connection_string(connection_string)
database_client = cosmos_client.get_database_client(db_name)
container_client = database_client.get_container_client(container_name)

data = {'key','value'}

container_client.upsert_item(data)
