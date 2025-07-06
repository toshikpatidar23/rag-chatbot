# rag-chatbot 
import os
  import asyncio
  from langchain_openai import OpenAIEmbeddings, ChatOpenAI
  from langchain.memory import ConversationBufferMemory
  from pinecone import Pinecone, ServerlessSpec, Index
  from langchain_pinecone import PineconeVectorStore
  from langchain.chains import create_history_aware_retriever, create_retrieval_chain, ConversationalRetrievalChain
  from langchain.prompts import PromptTemplate
  from dotenv import load_dotenv
