import React, { useEffect, useRef, useState } from "react";
import EmptyMassage from "./EmptyMassage";
import { LuPlus } from "react-icons/lu";
function App() {
  const getData = () => {
    let list = localStorage.getItem("task");
    return list ? JSON.parse(list) : [];
  };

  const [task, setTask] = useState(getData());
  const inputTask = useRef();

  const AddTask = () => {
    setTask([...task, { taskName: inputTask.current.value }]);
    inputTask.current.value = ""; // Clear input after adding a task
  };

  const DeleteTask = (index) => {
    const updatedTasks = task.filter((value, i) => index !== i);
    setTask(updatedTasks);
  };

  useEffect(() => {
    localStorage.setItem("task", JSON.stringify(task));
  }, [task]);

  return (
    <>
      <div className="min-h-screen bg-gradient-to-r from-blue-200 via-purple-200 to-pink-200 flex items-center justify-center px-4">
        <div className="w-full max-w-md bg-white rounded-lg shadow-md p-6">
          <div className="flex space-x-2 mb-4">
            <input
              ref={inputTask}
              type="text"
              className="flex-1 p-3 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-400 text-gray-700"
              placeholder="Enter a task"
            />
            <button
              className="px-6 py-3 bg-blue-500 text-white  rounded-md hover:bg-blue-600 hover:scale-105 transform transition-all duration-200"
              onClick={AddTask}
            >
             <LuPlus />
            </button>
          </div>
          {task.length === 0 ? (
            <EmptyMassage />
          ) : (
            <div className="space-y-2">
              {task.map((task, index) => (
                <div
                  className="flex items-center space-x-2 animate-fade-in"
                  key={index}
                >
                  <div className="p-3 flex-grow bg-blue-100 border border-blue-300 rounded-md text-blue-800">
                    {task.taskName}
                  </div>
                  <button
                    className="px-3 py-2 bg-red-500 text-white rounded-md hover:bg-red-600 hover:scale-105 transform transition-all duration-200"
                    onClick={() => DeleteTask(index)}
                  >
                    Delete
                  </button>
                </div>
              ))}
            </div>
          )}
        </div>
      </div>
    </>
  );
}

export default App;
