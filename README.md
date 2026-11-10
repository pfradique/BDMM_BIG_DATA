# BDMM_BIG_DATA
Big Data Modelling and Management

#terminal - passo 1
docker run -d \
  --name neo4j-server \
  -p 7474:7474 -p 7687:7687 \
  -v "$(pwd)/movie_data/databases:/data/databases" \
  -v "$(pwd)/movie_data/transactions:/data/transactions" \
  -e NEO4J_AUTH=neo4j/Neo4jneo4j \
  neo4j:community

# passo 2
pip install neo4j