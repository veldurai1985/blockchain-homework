# Proof of Authority Blockchain

1. Please find the screenshot the block chain tools folder before creating the PoA algorithum 

      ![Initial Folder](Images/initial_folder.jpg)

2. Screenshot of the genesis block. 

      ![Genesis Block 1](Images/genesis_1.jpg)

      ![Genesis Block 2](Images/genesis_2.jpg)

3. After genesis is created and nodes are activated, Nodes started commiting new mining work

    ![Node 1 Running](Images/node_1.jpg)

    ![Node 2 Running](Images/node_2.jpg)

4. After setting up the ETH network, I initiated the transaction. Please find the screen shot for the pending and successful transaction.

    Node 1 wallet:

    ![Node 1 Wallet](Images/Node1_Mywallet.jpg)

    Transaction in pending status:

    ![Pending Transaction](Images/pending.jpg)

    Successful transaction:

    ![Successful Transaction](Images/successful.jpg)


5. Please find the details about the private block chain network.

    * Network name: god

    * Chain ID / Number password: 2020

    * Node 1:

        password: god

        Public address of the key:   0xD163445F995F069a86ee2914de662962853F320A

        Path of the secret key file: node1\keystore\UTC--2020-10-21T23-46-23.377898100Z--d163445f995f069a86ee2914de662962853f320a

        enode://6a50f80b9fa15ef8d1eafbc1ca3bcd438792e54bead32a700487deda10e3ff0be18ec23119b7b746e198be0da952c7cdd5b52a2f56b87272f0fcef933fc034c5@127.0.0.1:30303


    * Node 2:
    
        Repeat password: god

        Public address of the key:   0x470Ffdf8d4Db502f8f4F0980E303916B4Be7A1aa

        Path of the secret key file: node2\keystore\UTC--2020-10-21T23-47-59.633430300Z--470ffdf8d4db502f8f4f0980e303916b4be7a1aa

6. Instruction to activate node1 and node2.

    * Run the nodes in separate terminal windows with the commands:
        *  ./geth --datadir node1 --unlock "0xD163445F995F069a86ee2914de662962853F320A" --mine --rpc --allow-insecure-unlock
        *  ./geth --datadir node2 --unlock "0x470Ffdf8d4Db502f8f4F0980E303916B4Be7A1aa" --mine --port 30304 --bootnodes "enode://6a50f80b9fa15ef8d1eafbc1ca3bcd438792e54bead32a700487deda10e3ff0be18ec23119b7b746e198be0da952c7cdd5b52a2f56b87272f0fcef933fc034c5@127.0.0.1:30303" --ipcdisable --allow-insecure-unlock

        Node 1 Restart:

        ![Node 1 restart](Images/node1_restart.jpg)

        Node 2 Restart:

        ![Node 2 restart](Images/node1_restart.jpg)
