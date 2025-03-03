import { motion } from "framer-motion";

export default function AnimatedCharacter() {
  return (
    <div className="flex flex-col items-center justify-center h-screen bg-gray-100">
      <motion.div
        className="relative flex flex-col items-center"
      >
        {/* Girl */}
        <motion.div
          className="w-32 h-32 bg-pink-400 rounded-full flex items-center justify-center text-white text-3xl font-bold"
          animate={{ y: [0, -5, 0] }}
          transition={{ repeat: Infinity, duration: 1, ease: "easeInOut" }}
        >
      
  <img src="/girl.png" alt="Little Girl" className="w-full h-full object-cover" />


        </motion.div>

        {/* Arm writing animation */}
        <motion.div
          className="absolute top-16 left-8 w-16 h-4 bg-brown-500 rounded"
          animate={{ rotate: [0, -10, 0, 10, 0] }}
          transition={{ repeat: Infinity, duration: 1.5, ease: "easeInOut" }}
        >
        
  <img src="/arm.png" alt="Arm" className="w-full h-full" />


        </motion.div>

        {/* Paper */}
        <motion.div
          className="mt-16 w-32 h-24 bg-white border border-gray-400 rounded shadow-lg"
        >
        <img src="/paper.png" alt="Paper" className="w-full h-full object-contain" />
        </motion.div>
      </motion.div>
    </div>
  );
}
