FROM trufflesuite/ganache:latest

# Expose the standard port used in your application
EXPOSE 7545

# Start Ganache on 0.0.0.0 so it can be accessed externally
# We also inject the exact private key used in your Spring Boot application with 1000 ETH
ENTRYPOINT ["node", "/app/dist/node/cli.js", "--server.host", "0.0.0.0", "--server.port", "7545", "--wallet.accounts=0xe0396dd66930d63f462627faa75345913890d5476f4441b2bfb639a8a838f51f,1000000000000000000000"]
