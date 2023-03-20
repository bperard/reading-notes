# 428

## useEffect hook

- What is the main intended use case for the useEffect hook?  
Call useEffect at the top level of your component to declare an Effect.

- How does the effect’s logic interact with the component?  
When your component is first added to the DOM, React will run your setup function. After every re-render with changed dependencies, React will first run the cleanup function (if you provided it) with the old values, and then run your setup function with the new values. After your component is removed from the DOM, React will run your cleanup function one last time.

- What is the importance of the return value from the effect’s logic function?  
It should return a cleanup function with cleanup code that disconnects from that system.
